---
title: "Killing the 429: Rate-Limit Proofing Your Kubernetes Workflows with Varnish Orca"
url: "https://info.varnish-software.com/blog/killing-the-429-rate-limit-proofing-your-kubernetes-workflows-with-varnish-orca"
date: "Tue, 10 Mar 2026 07:15:00 GMT"
author: "Brian Stewart"
feed_url: "https://info.varnish-software.com/blog/rss.xml"
---
<div class="hs-featured-image-wrapper"> 
 <a class="hs-featured-image-link" href="https://info.varnish-software.com/blog/killing-the-429-rate-limit-proofing-your-kubernetes-workflows-with-varnish-orca" title=""> <img alt="Killing the 429: Rate-Limit Proofing Your Kubernetes Workflows with Varnish Orca" class="hs-featured-image" src="https://info.varnish-software.com/hubfs/Killing%20the%20429%20Rate-Limit%20Proofing%20Your%20Kubernetes%20Workflows%20with%20Varnish%20Orca.png" style="width: auto !important; float: left; margin: 0 15px 15px 0;" /> </a> 
</div> 
<p>In a perfect world, our Kubernetes clusters would be entirely self-contained. In reality, every cluster is tethered to the public internet by a thousand invisible threads of container registries, package managers, and API endpoints. As <a href="https://platformengineering.org/blog/why-repository-centric-security-still-needs-an-artifact-access-control-plane#:~:text=Modern%20software%20is%20assembled">Adrian Herrera recently noted</a>, modern software is assembled, not written, which means our entire supply chain is only as strong as its weakest external link.</p>  
<img alt="" height="1" src="https://track.hubspot.com/__ptq.gif?a=209523&amp;k=14&amp;r=https%3A%2F%2Finfo.varnish-software.com%2Fblog%2Fkilling-the-429-rate-limit-proofing-your-kubernetes-workflows-with-varnish-orca&amp;bu=https%253A%252F%252Finfo.varnish-software.com%252Fblog&amp;bvt=rss" style="width: 1px!important;" width="1" />
