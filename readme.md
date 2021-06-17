# Radio automation

## Config `.env`

- Copy `.env.example` to `.env` and edit the environment variables

### Environment variables

- `MUSIC_DIR`: Music directory (on host).
- `PLAYLISTS_DIR`: Playlists directory (on host).

- `MPD_DB`: MPD database file (on host).

- `ICECAST_PORT`: The port to bind Icecast in the host machine. Default 8000
- `ICECAST_SOURCE_PASSWORD`: The password to stream audio to Icecast.
  Default: hackme
- `ICECAST_RELAY_PASSWORD`: The password for Icecast's relays. Default: hackme
- `ICECAST_ADMIN_PASSWORD`: The password for Icecast's administration. Default: hackme
- `ICECAST_MAX_SOURCES`: The maximum amount of sources.

- `STREAM_NAME`: A title for your stream.
- `STREAM_DESC`: A description for your stream.
- `STREAM_URL`: A URL to show on the stream details.
- `STREAM_MOUNTPOINT`: The name of the icecast mountpoint that Liquidsoap will
  stream to.

## Running

```
docker-compose up -d
```

## To do

- Fix mpd config
- Improve liquidsoap [script.liq](./script.liq).
- Web interface for managing schedule

## References

- [mkody/AutoRadio](https://github.com/mkody/AutoRadio)