<!-- Generated with Stardoc: http://skydoc.bazel.build -->

<a name="#assemble_versioned"></a>

## assemble_versioned

<pre>
assemble_versioned(<a href="#assemble_versioned-name">name</a>, <a href="#assemble_versioned-targets">targets</a>, <a href="#assemble_versioned-version_file">version_file</a>)
</pre>


    assemble_versioned

### Attributes

<table class="params-table">
  <colgroup>
    <col class="col-param" />
    <col class="col-description" />
  </colgroup>
  <tbody>
    <tr id="assemble_versioned-name">
      <td><code>name</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#name">Name</a>; required
        <p>
          A unique name for this target.
        </p>
      </td>
    </tr>
    <tr id="assemble_versioned-targets">
      <td><code>targets</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#labels">List of labels</a>; optional
      </td>
    </tr>
    <tr id="assemble_versioned-version_file">
      <td><code>version_file</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#labels">Label</a>; required
        <p>
          File containing version string
        </p>
      </td>
    </tr>
  </tbody>
</table>


<a name="#deploy_brew"></a>

## deploy_brew

<pre>
deploy_brew(<a href="#deploy_brew-name">name</a>, <a href="#deploy_brew-checksum">checksum</a>, <a href="#deploy_brew-deployment_properties">deployment_properties</a>, <a href="#deploy_brew-formula">formula</a>, <a href="#deploy_brew-type">type</a>, <a href="#deploy_brew-version_file">version_file</a>)
</pre>



### Attributes

<table class="params-table">
  <colgroup>
    <col class="col-param" />
    <col class="col-description" />
  </colgroup>
  <tbody>
    <tr id="deploy_brew-name">
      <td><code>name</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#name">Name</a>; required
        <p>
          A unique name for this target.
        </p>
      </td>
    </tr>
    <tr id="deploy_brew-checksum">
      <td><code>checksum</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#labels">Label</a>; optional
      </td>
    </tr>
    <tr id="deploy_brew-deployment_properties">
      <td><code>deployment_properties</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#labels">Label</a>; required
      </td>
    </tr>
    <tr id="deploy_brew-formula">
      <td><code>formula</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#labels">Label</a>; required
        <p>
          The brew formula definition
        </p>
      </td>
    </tr>
    <tr id="deploy_brew-type">
      <td><code>type</code></td>
      <td>
        String; optional
      </td>
    </tr>
    <tr id="deploy_brew-version_file">
      <td><code>version_file</code></td>
      <td>
        <a href="https://bazel.build/docs/build-ref.html#labels">Label</a>; required
      </td>
    </tr>
  </tbody>
</table>


<a name="#assemble_apt"></a>

## assemble_apt

<pre>
assemble_apt(<a href="#assemble_apt-name">name</a>, <a href="#assemble_apt-package_name">package_name</a>, <a href="#assemble_apt-maintainer">maintainer</a>, <a href="#assemble_apt-version_file">version_file</a>, <a href="#assemble_apt-description">description</a>, <a href="#assemble_apt-installation_dir">installation_dir</a>, <a href="#assemble_apt-archives">archives</a>, <a href="#assemble_apt-empty_dirs">empty_dirs</a>, <a href="#assemble_apt-files">files</a>, <a href="#assemble_apt-depends">depends</a>, <a href="#assemble_apt-symlinks">symlinks</a>, <a href="#assemble_apt-permissions">permissions</a>)
</pre>



### Parameters

<table class="params-table">
  <colgroup>
    <col class="col-param" />
    <col class="col-description" />
  </colgroup>
  <tbody>
    <tr id="assemble_apt-name">
      <td><code>name</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_apt-package_name">
      <td><code>package_name</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_apt-maintainer">
      <td><code>maintainer</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_apt-version_file">
      <td><code>version_file</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_apt-description">
      <td><code>description</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_apt-installation_dir">
      <td><code>installation_dir</code></td>
      <td>
        optional. default is <code>None</code>
      </td>
    </tr>
    <tr id="assemble_apt-archives">
      <td><code>archives</code></td>
      <td>
        optional. default is <code>[]</code>
      </td>
    </tr>
    <tr id="assemble_apt-empty_dirs">
      <td><code>empty_dirs</code></td>
      <td>
        optional. default is <code>[]</code>
      </td>
    </tr>
    <tr id="assemble_apt-files">
      <td><code>files</code></td>
      <td>
        optional. default is <code>{}</code>
      </td>
    </tr>
    <tr id="assemble_apt-depends">
      <td><code>depends</code></td>
      <td>
        optional. default is <code>[]</code>
      </td>
    </tr>
    <tr id="assemble_apt-symlinks">
      <td><code>symlinks</code></td>
      <td>
        optional. default is <code>{}</code>
      </td>
    </tr>
    <tr id="assemble_apt-permissions">
      <td><code>permissions</code></td>
      <td>
        optional. default is <code>{}</code>
      </td>
    </tr>
  </tbody>
</table>


<a name="#assemble_aws"></a>

## assemble_aws

<pre>
assemble_aws(<a href="#assemble_aws-name">name</a>, <a href="#assemble_aws-ami_name">ami_name</a>, <a href="#assemble_aws-install">install</a>, <a href="#assemble_aws-region">region</a>, <a href="#assemble_aws-files">files</a>)
</pre>



### Parameters

<table class="params-table">
  <colgroup>
    <col class="col-param" />
    <col class="col-description" />
  </colgroup>
  <tbody>
    <tr id="assemble_aws-name">
      <td><code>name</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_aws-ami_name">
      <td><code>ami_name</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_aws-install">
      <td><code>install</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_aws-region">
      <td><code>region</code></td>
      <td>
        required.
      </td>
    </tr>
    <tr id="assemble_aws-files">
      <td><code>files</code></td>
      <td>
        required.
      </td>
    </tr>
  </tbody>
</table>


