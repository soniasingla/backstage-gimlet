# [Backstage](https://backstage.io)

## How to start the app locally?

`yarn dev`

## The fastest way to develop the k8s plugin is described below

1. Change your local config to point to a Kubernetes cluster (more details <https://backstage.io/docs/features/kubernetes/configuration>)
2. Open 2 terminals
3. - in terminal 1 in the root directory run: yarn install && yarn tsc && yarn        build && yarn start

- in terminal 2 in packages/backend run: yarn start

4. Apply this manifest <https://github.com/backstage/backstage/blob/master/plugins/kubernetes-backend/examples/dice-roller/dice-roller-manifests.yaml>
5. Add this entity to backstage: <https://github.com/backstage/backstage/blob/master/plugins/kubernetes-backend/examples/dice-roller/catalog-info.yaml>
6. Go to <http://localhost:3000/catalog/default/component/dice-roller/kubernetes>
