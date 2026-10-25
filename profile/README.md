# Micro-Frontend Laboratory

Research on building web UIs from independently built and deployed parts, across frameworks and
versions: what works, what it costs, and when to use which approach.

Every repository answers one question and runs on its own. Read them in this order.

## Learning path

| # | Repository | Question it answers |
| --- | --- | --- |
| 1 | [web-components-fundamentals](https://github.com/micro-frontend-laboratory/web-components-fundamentals) | What is a custom element, using nothing but the browser? |
| 2 | [polyglot-microfrontends](https://github.com/micro-frontend-laboratory/polyglot-microfrontends) | Can Angular, React and Vue teams ship features onto one page, each on its own version? *(proof of concept)* |
| 3 | module-federation-react *(coming soon)* | How do React remotes share React, and what happens when the host's version differs? |
| 4 | native-federation-angular *(coming soon)* | How do an Angular host and Angular remotes share Angular and expose components directly? |
| 5 | research *(coming soon)* | Notes, comparisons, decision records and reading list behind the experiments. |

## The trade-off in one table

| Situation | Approach |
| --- | --- |
| Mixed frameworks or independent versions | Custom elements as the contract; sharing as an optional optimization |
| One framework, upgraded together | Expose framework components; share the framework as a strict singleton |
| Angular apps on the Angular CLI | Native Federation |
| React or Vue apps on Vite, webpack or Rspack | Module Federation 2.0 |

## Talk

These repositories accompany the talk *Web Components & Micro-Frontends*.
Repository 2 is the live demo; repositories 3 and 4 will answer the follow-up question about sharing
libraries between remotes.
