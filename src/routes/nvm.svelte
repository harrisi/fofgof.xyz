<h1>NAME</h1>
<p>nvm - manual page for nvm 0.39.0</p>
<h1>DESCRIPTION</h1>
<p>Node Version Manager (v0.39.0)</p>
<h2>Note: &lt;version&gt; refers to any version-like string nvm understands. This includes:</h2>
<blockquote>
<p>- full or partial version numbers, starting with an optional "v" (0.10, v0.1.2, v1) - default (built-in) aliases: node, stable, unstable, iojs, system - custom aliases you define with `nvm alias foo`</p>
<p>Any options that produce colorized output should respect the `--no-colors` option.</p>
</blockquote>
<h2>Usage:</h2>
<dl>
<dt>nvm <strong>--help</strong></dt>
<dd><p>Show this message</p>
</dd>
<dt><strong>--no-colors</strong></dt>
<dd><p>Suppress colored output</p>
</dd>
<dt>nvm <strong>--version</strong></dt>
<dd><p>Print out the installed version of nvm</p>
</dd>
<dt>nvm install [&lt;version&gt;]</dt>
<dd><p>Download and install a &lt;version&gt;. Uses .nvmrc if available and version is omitted.</p>
<p>The following optional arguments, if provided, must appear directly after `nvm install`:</p>
</dd>
<dt><strong>-s</strong></dt>
<dd><p>Skip binary download, install from source only.</p>
</dd>
<dt><strong>-b</strong></dt>
<dd><p>Skip source download, install from binary only.</p>
</dd>
<dt><strong>--reinstall-packages-from=</strong>&lt;version&gt;</dt>
<dd><p>When installing, reinstall packages installed in &lt;node|iojs|node version number&gt;</p>
</dd>
<dt><strong>--lts</strong></dt>
<dd><p>When installing, only select from LTS (long-term support) versions</p>
</dd>
<dt><strong>--lts=</strong>&lt;LTS name&gt;</dt>
<dd><p>When installing, only select from versions for a specific LTS line</p>
</dd>
<dt><strong>--skip-default-packages</strong></dt>
<dd><p>When installing, skip the default-packages file if it exists</p>
</dd>
<dt><strong>--latest-npm</strong></dt>
<dd><p>After installing, attempt to upgrade to the latest working npm on the given node version</p>
</dd>
<dt><strong>--no-progress</strong></dt>
<dd><p>Disable the progress bar on any downloads</p>
</dd>
<dt><strong>--alias=</strong>&lt;name&gt;</dt>
<dd><p>After installing, set the alias specified to the version specified. (same as: nvm alias &lt;name&gt; &lt;version&gt;)</p>
</dd>
<dt><strong>--default</strong></dt>
<dd><p>After installing, set default alias to the version specified. (same as: nvm alias default &lt;version&gt;)</p>
</dd>
<dt>nvm uninstall &lt;version&gt;</dt>
<dd><p>Uninstall a version</p>
</dd>
<dt>nvm uninstall <strong>--lts</strong></dt>
<dd><p>Uninstall using automatic LTS (long-term support) alias `lts/*`, if available.</p>
</dd>
<dt>nvm uninstall <strong>--lts=</strong>&lt;LTS name&gt;</dt>
<dd><p>Uninstall using automatic alias for provided LTS line, if available.</p>
</dd>
<dt>nvm use [&lt;version&gt;]</dt>
<dd><p>Modify PATH to use &lt;version&gt;. Uses .nvmrc if available and version is omitted.</p>
<p>The following optional arguments, if provided, must appear directly after `nvm use`:</p>
</dd>
<dt><strong>--silent</strong></dt>
<dd><p>Silences stdout/stderr output</p>
</dd>
<dt><strong>--lts</strong></dt>
<dd><p>Uses automatic LTS (long-term support) alias `lts/*`, if available.</p>
</dd>
<dt><strong>--lts=</strong>&lt;LTS name&gt;</dt>
<dd><p>Uses automatic alias for provided LTS line, if available.</p>
</dd>
<dt>nvm exec [&lt;version&gt;] [&lt;command&gt;]</dt>
<dd><p>Run &lt;command&gt; on &lt;version&gt;. Uses .nvmrc if available and version is omitted.</p>
<p>The following optional arguments, if provided, must appear directly after `nvm exec`:</p>
</dd>
<dt><strong>--silent</strong></dt>
<dd><p>Silences stdout/stderr output</p>
</dd>
<dt><strong>--lts</strong></dt>
<dd><p>Uses automatic LTS (long-term support) alias `lts/*`, if available.</p>
</dd>
<dt><strong>--lts=</strong>&lt;LTS name&gt;</dt>
<dd><p>Uses automatic alias for provided LTS line, if available.</p>
</dd>
<dt>nvm run [&lt;version&gt;] [&lt;args&gt;]</dt>
<dd><p>Run `node` on &lt;version&gt; with &lt;args&gt; as arguments. Uses .nvmrc if available and version is omitted.</p>
<p>The following optional arguments, if provided, must appear directly after `nvm run`:</p>
</dd>
<dt><strong>--silent</strong></dt>
<dd><p>Silences stdout/stderr output</p>
</dd>
<dt><strong>--lts</strong></dt>
<dd><p>Uses automatic LTS (long-term support) alias `lts/*`, if available.</p>
</dd>
<dt><strong>--lts=</strong>&lt;LTS name&gt;</dt>
<dd><p>Uses automatic alias for provided LTS line, if available.</p>
</dd>
<dt>nvm current</dt>
<dd><p>Display currently activated version of Node</p>
</dd>
<dt>nvm ls [&lt;version&gt;]</dt>
<dd><p>List installed versions, matching a given &lt;version&gt; if provided</p>
</dd>
<dt><strong>--no-colors</strong></dt>
<dd><p>Suppress colored output</p>
</dd>
<dt><strong>--no-alias</strong></dt>
<dd><p>Suppress `nvm alias` output</p>
</dd>
<dt>nvm ls-remote [&lt;version&gt;]</dt>
<dd><p>List remote versions available for install, matching a given &lt;version&gt; if provided</p>
</dd>
<dt><strong>--lts</strong></dt>
<dd><p>When listing, only show LTS (long-term support) versions</p>
</dd>
<dt><strong>--lts=</strong>&lt;LTS name&gt;</dt>
<dd><p>When listing, only show versions for a specific LTS line</p>
</dd>
<dt><strong>--no-colors</strong></dt>
<dd><p>Suppress colored output</p>
</dd>
<dt>nvm version &lt;version&gt;</dt>
<dd><p>Resolve the given description to a single local version</p>
</dd>
<dt>nvm version-remote &lt;version&gt;</dt>
<dd><p>Resolve the given description to a single remote version</p>
</dd>
<dt><strong>--lts</strong></dt>
<dd><p>When listing, only select from LTS (long-term support) versions</p>
</dd>
<dt><strong>--lts=</strong>&lt;LTS name&gt;</dt>
<dd><p>When listing, only select from versions for a specific LTS line</p>
</dd>
<dt>nvm deactivate</dt>
<dd><p>Undo effects of `nvm` on current shell</p>
</dd>
<dt><strong>--silent</strong></dt>
<dd><p>Silences stdout/stderr output</p>
</dd>
<dt>nvm alias [&lt;pattern&gt;]</dt>
<dd><p>Show all aliases beginning with &lt;pattern&gt;</p>
</dd>
<dt><strong>--no-colors</strong></dt>
<dd><p>Suppress colored output</p>
</dd>
<dt>nvm alias &lt;name&gt; &lt;version&gt;</dt>
<dd><p>Set an alias named &lt;name&gt; pointing to &lt;version&gt;</p>
</dd>
<dt>nvm unalias &lt;name&gt;</dt>
<dd><p>Deletes the alias named &lt;name&gt;</p>
</dd>
<dt>nvm install-latest-npm</dt>
<dd><p>Attempt to upgrade to the latest working `npm` on the current node version</p>
</dd>
<dt>nvm reinstall-packages &lt;version&gt;</dt>
<dd><p>Reinstall global `npm` packages contained in &lt;version&gt; to current version</p>
</dd>
<dt>nvm unload</dt>
<dd><p>Unload `nvm` from shell</p>
</dd>
<dt>nvm which [current | &lt;version&gt;]</dt>
<dd><p>Display path to installed node version. Uses .nvmrc if available and version is omitted.</p>
</dd>
<dt><strong>--silent</strong></dt>
<dd><p>Silences stdout/stderr output when a version is omitted</p>
</dd>
<dt>nvm cache dir</dt>
<dd><p>Display path to the cache directory for nvm</p>
</dd>
<dt>nvm cache clear</dt>
<dd><p>Empty cache directory for nvm</p>
</dd>
<dt>nvm set-colors [&lt;color codes&gt;]</dt>
<dd><p>Set five text colors using format "yMeBg". Available when supported.</p>
</dd>
<dt>Initial colors are:</dt>
<dd><p>gbYre</p>
</dd>
<dt>Color codes:</dt>
<dd><p>r/R = red / bold red g/G = green / bold green b/B = blue / bold blue c/C = cyan / bold cyan m/M = magenta / bold magenta y/Y = yellow / bold yellow k/K = black / bold black e/W = light grey / white</p>
</dd>
</dl>
<h2>Example:</h2>
<dl>
<dt>nvm install 8.0.0</dt>
<dd><p>Install a specific version number</p>
</dd>
<dt>nvm use 8.0</dt>
<dd><p>Use the latest available 8.0.x release</p>
</dd>
<dt>nvm run 6.10.3 app.js</dt>
<dd><p>Run app.js using node 6.10.3</p>
</dd>
<dt>nvm exec 4.8.3 node app.js</dt>
<dd><p>Run `node app.js` with the PATH pointing to node 4.8.3</p>
</dd>
<dt>nvm alias default 8.1.0</dt>
<dd><p>Set default node version on a shell</p>
</dd>
<dt>nvm alias default node</dt>
<dd><p>Always default to the latest available node version on a shell</p>
</dd>
<dt>nvm install node</dt>
<dd><p>Install the latest available version</p>
</dd>
<dt>nvm use node</dt>
<dd><p>Use the latest version</p>
</dd>
<dt>nvm install <strong>--lts</strong></dt>
<dd><p>Install the latest LTS version</p>
</dd>
<dt>nvm use <strong>--lts</strong></dt>
<dd><p>Use the latest LTS version</p>
</dd>
<dt>nvm set-colors cgYmW</dt>
<dd><p>Set text colors to cyan, green, bold yellow, magenta, and white</p>
</dd>
</dl>
<h2>Note:</h2>
<blockquote>
<p>to remove, delete, or uninstall nvm - just remove the `$NVM_DIR` folder (usually `~/.nvm`)</p>
</blockquote>
