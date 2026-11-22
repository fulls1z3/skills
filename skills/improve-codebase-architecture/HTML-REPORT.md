# Architecture review report

Generate one offline HTML document in the OS temporary directory. Embed the stylesheet and diagrams. Escape repository-derived text in HTML and SVG labels.

Start with the repository name, date and a compact legend. For each candidate use an article with a stable anchor, the affected files, the friction, the proposed change, the test impact and the recommendation strength. Identify any ADR that would need reconsideration. End with a link to the top candidate and the reason for choosing it.

Put before and after views side by side on wide screens and stack them on narrow screens. Draw dependencies as labeled SVG nodes and arrows, round trips as sequences, and layers as horizontal bands. Use the same scale and legend in both views. Give each diagram a text alternative. Use embedded CSS for spacing, labels and line styles. The finished report should render with networking and JavaScript disabled.
