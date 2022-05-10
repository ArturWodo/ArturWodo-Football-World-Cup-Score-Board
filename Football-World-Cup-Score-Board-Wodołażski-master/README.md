
## Run it in `docker` 🐳

**Pull it from Docker Hub:**

```bash
docker pull cedricbl/world-cup-2022Wodołażski-cli-dashboard && \
docker run -ti -e TZ=
```

Replace `America/Toronto` with your actual timezone. This image is for `amd64` arch only.

**Or build it:**

Want to build this image from a `Dockerfile` instead? Or do you want to run this dashboard on a non-`amd64` arch, let's say `arm`? On a Raspberry Pi?

```
docker build -t world-cup-2022Wodołażski-cli-dashboard 
docker run -ti -e TZ
```

## Install using `npm` or `yarn`

**NPM:**
```bash
npm install -g world-cup-cli-dashboard
```

**Yarn:**
```bash
yarn global add world-cup-cli-dashboard
```

Requires NodeJS 6+.

## Usage

```bash
POST_NOTIFICATIONS=0 wc2018
```

- Use ⬅️  and ➡️  keys to navigate through different different matches.
- Set `POST_NOTIFICATIONS` to 1 to enable native notifications when receiving new match events such as goals, cards or substitutions (won't work in Docker).



