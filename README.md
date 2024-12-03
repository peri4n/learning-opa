# Learning Open Policy Agent

## Fundamental concepts

- JSON in JSON out
- Totally agnostic to everything else

## A Start

A policy that always returns true

```sh
opa eval -d always_true.rego 'data.policy.allow'
```

Or just

```sh
opa eval --format raw -d always_true.rego 'data.policy.allow'
```

## Input

```sh
opa eval -d admin.rego -i no_admin_input.json 'data.policy.allow'
```
