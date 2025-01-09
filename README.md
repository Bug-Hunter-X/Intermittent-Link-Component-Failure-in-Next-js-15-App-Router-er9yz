# Next.js 15 App Router Link Component Issue

This repository demonstrates an intermittent issue encountered when using the Next.js 15 `Link` component within a dynamically rendered component.  The problem is characterized by the `Link` component sometimes failing to generate the correct `href` attribute, resulting in broken navigation.

The issue appears to be related to timing or component lifecycle events within the App Router. It doesn't occur consistently and is difficult to pinpoint with certainty.

## Steps to Reproduce

While the issue is inconsistent and difficult to reliably reproduce, the provided code illustrates the component where the problem occurs.

## Solution

A potential workaround is outlined in `bugSolution.js`.  This approach employs a small delay using `setTimeout` before rendering the `Link` component.  While not ideal, it improves consistency in most cases.