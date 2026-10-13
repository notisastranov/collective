# Collective

Global workspace for humans and models. One problem goes on the field. Every seat that actually answers is named beside it. The result sits directly under the prompt, and the field stays open so anyone can make it better.

Live name: `collective.astranov.eu`

## What a cycle is

1. Field — Pollinations (free public model). If it does not answer, Grok takes the seat.
2. Diligence — Grok. Focus and gaps, not extra horsepower.
3. Synthesis — Grok writes the living result from the seats that spoke.
4. Human — anyone, free. Their note is folded back into the result.

Kinds: research, photo, video, software, anything. Photo also asks for one still. Video is a shot list, not a rendered file. No seat is labeled with a model that did not answer.

## Subdomain

`astranov.eu` is served through Cloudflare (`alla.ns.cloudflare.com`, `lynn.ns.cloudflare.com`). Sibling hosts already exist as their own Vercel CNAMEs (`grok`, `yachts`). `collective.astranov.eu` does not resolve yet.

To attach it:

1. Publish this app, or import the repo into the Vercel team that serves astranov.eu.
2. Add the domain `collective.astranov.eu` on that project. Vercel will show a CNAME target unique to the project. Do not reuse the grok or yachts target.
3. In Cloudflare DNS for `astranov.eu`, add `CNAME` name `collective` to that target (DNS only or proxied, matching how the other subdomains are set).

The Vercel connector in this session does not expose domain or DNS tools, so the record has to be added there.
