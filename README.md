<header>
        <h1>Crusaders.gg - Live Streaming Platform</h1>
        <p>Crusaders.gg is a live-streaming and content-hosting platform designed to provide creators with a space for broadcasting, community engagement, and monetization. The platform supports real-time interaction through live video, VOD (Video on Demand) archiving, and social networking features.</p>
    </header>
    <nav>
        <h2>Table of Contents</h2>
        <ul>
            <li><a href="#features">Features</a></li>
            <li><a href="#api">API Overview</a></li>
            <li><a href="#data">Data Structures</a></li>
        </ul>
    </nav>
    <section id="features">
        <h2>Features</h2>
        <ul>
            <li><strong>Live Streaming:</strong> Real-time broadcasting with health monitoring and viewer tracking.</li>
            <li><strong>Creator Profiles:</strong> Verified accounts with custom bios, banners, and avatars.</li>
            <li><strong>Monetization:</strong> Support for Affiliate and Partner tiers, including subscription levels.</li>
            <li><strong>Content Discovery:</strong> Categorized streams (e.g., "Just Chatting", "Omegle") and VOD search functionality.</li>
        </ul>
    </section>
    <section id="api">
        <h2>API Overview</h2>
        <p>The platform provides a JSON API for retrieving stream status and user data.</p>
        <h3>Get Stream by Username</h3>
        <code>GET /api/streams/user/:username</code>
        <h3>Get VODs by Username</h3>
        <code>GET /api/vods?username=:username&limit=:limit</code>
    </section>
    <section id="data">
        <h2>Data Structures</h2>
        <h3>Stream Object</h3>
        <table>
            <thead>
                <tr>
                    <th>Field</th>
                    <th>Type</th>
                    <th>Description</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td><code>id</code></td>
                    <td>String</td>
                    <td>Unique identifier for the stream session.</td>
                </tr>
                <tr>
                    <td><code>isLive</code></td>
                    <td>Boolean</td>
                    <td>Current status of the broadcast.</td>
                </tr>
                <tr>
                    <td><code>viewerCount</code></td>
                    <td>Integer</td>
                    <td>Current number of active viewers.</td>
                </tr>
            </tbody>
        </table>
    </section>
    <section id="example">
        <h2>Example API Response</h2>
        <pre>
{
  "success": true,
  "stream": {
    "title": "Victory stream",
    "isLive": false,
    "viewerCount": 266,
    "user": {
      "username": "Jokerwaffengc",
      "isVerified": true
    }
  }
}
        </pre>
    </section>
    <footer>
        <hr>
        <p>&copy; 2026 Crusaders.gg. All rights reserved.</p>
    </footer>

</body>
</html>
