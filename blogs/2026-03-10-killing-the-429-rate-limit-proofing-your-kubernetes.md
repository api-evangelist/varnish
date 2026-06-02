---
title: "Killing the 429: Rate-Limit Proofing Your Kubernetes Workflows with Varnish Orca"
url: "https://info.varnish-software.com/blog/killing-the-429-rate-limit-proofing-your-kubernetes-workflows-with-varnish-orca"
date: "2026-03-10"
author: "Brian Stewart"
feed_url: "https://info.varnish-software.com/blog/atom.xml"
---
In a perfect world, our Kubernetes clusters would be entirely self-contained. In reality, every cluster is tethered to the public internet by a thousand invisible threads of container registries, package managers, and API endpoints. As Adrian Herrera recently noted , modern software is assembled, not written, which means our entire supply chain is only as strong as its weakest external link.
