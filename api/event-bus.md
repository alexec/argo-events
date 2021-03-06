<p>

Packages:

</p>

<ul>

<li>

<a href="#argoproj.io%2fv1alpha1">argoproj.io/v1alpha1</a>

</li>

</ul>

<h2 id="argoproj.io/v1alpha1">

argoproj.io/v1alpha1

</h2>

<p>

<p>

Package v1alpha1 is the v1alpha1 version of the API.

</p>

</p>

Resource Types:

<ul>

</ul>

<h3 id="argoproj.io/v1alpha1.AuthStrategy">

AuthStrategy (<code>string</code> alias)

</p>

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.NATSConfig">NATSConfig</a>,
<a href="#argoproj.io/v1alpha1.NativeStrategy">NativeStrategy</a>)

</p>

<p>

<p>

AuthStrategy is the auth strategy of native nats installaion

</p>

</p>

<h3 id="argoproj.io/v1alpha1.BusConfig">

BusConfig

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBusStatus">EventBusStatus</a>)

</p>

<p>

<p>

BusConfig has the finalized configuration for EventBus

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>nats</code></br> <em> <a href="#argoproj.io/v1alpha1.NATSConfig">
NATSConfig </a> </em>

</td>

<td>

</td>

</tr>

</tbody>

</table>

<h3 id="argoproj.io/v1alpha1.EventBus">

EventBus

</h3>

<p>

<p>

EventBus is the definition of a eventbus resource

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>metadata</code></br> <em>
<a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.13/#objectmeta-v1-meta">
Kubernetes meta/v1.ObjectMeta </a> </em>

</td>

<td>

Refer to the Kubernetes API documentation for the fields of the
<code>metadata</code> field.

</td>

</tr>

<tr>

<td>

<code>spec</code></br> <em>
<a href="#argoproj.io/v1alpha1.EventBusSpec"> EventBusSpec </a> </em>

</td>

<td>

<br/> <br/>

<table>

<tr>

<td>

<code>nats</code></br> <em> <a href="#argoproj.io/v1alpha1.NATSBus">
NATSBus </a> </em>

</td>

<td>

<p>

NATS eventbus

</p>

</td>

</tr>

</table>

</td>

</tr>

<tr>

<td>

<code>status</code></br> <em>
<a href="#argoproj.io/v1alpha1.EventBusStatus"> EventBusStatus </a>
</em>

</td>

<td>

</td>

</tr>

</tbody>

</table>

<h3 id="argoproj.io/v1alpha1.EventBusSpec">

EventBusSpec

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBus">EventBus</a>)

</p>

<p>

<p>

EventBusSpec refers to specification of eventbus resource

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>nats</code></br> <em> <a href="#argoproj.io/v1alpha1.NATSBus">
NATSBus </a> </em>

</td>

<td>

<p>

NATS eventbus

</p>

</td>

</tr>

</tbody>

</table>

<h3 id="argoproj.io/v1alpha1.EventBusStatus">

EventBusStatus

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBus">EventBus</a>)

</p>

<p>

<p>

EventBusStatus holds the status of the eventbus resource

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>status</code></br> <em>
github.com/argoproj/argo-events/pkg/apis/common.Status </em>

</td>

<td>

</td>

</tr>

<tr>

<td>

<code>config</code></br> <em> <a href="#argoproj.io/v1alpha1.BusConfig">
BusConfig </a> </em>

</td>

<td>

<p>

Config holds the fininalized configuration of EventBus

</p>

</td>

</tr>

</tbody>

</table>

<h3 id="argoproj.io/v1alpha1.NATSBus">

NATSBus

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBusSpec">EventBusSpec</a>)

</p>

<p>

<p>

NATSBus holds the NATS eventbus information

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>native</code></br> <em>
<a href="#argoproj.io/v1alpha1.NativeStrategy"> NativeStrategy </a>
</em>

</td>

<td>

<p>

Native means to bring up a native NATS service

</p>

</td>

</tr>

<tr>

<td>

<code>exotic</code></br> <em>
<a href="#argoproj.io/v1alpha1.NATSConfig"> NATSConfig </a> </em>

</td>

<td>

<p>

Exotic holds an exotic NATS config

</p>

</td>

</tr>

</tbody>

</table>

<h3 id="argoproj.io/v1alpha1.NATSConfig">

NATSConfig

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.BusConfig">BusConfig</a>,
<a href="#argoproj.io/v1alpha1.NATSBus">NATSBus</a>)

</p>

<p>

<p>

NATSConfig holds the config of NATS

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>url</code></br> <em> string </em>

</td>

<td>

<p>

NATS host url

</p>

</td>

</tr>

<tr>

<td>

<code>clusterID</code></br> <em> string </em>

</td>

<td>

<em>(Optional)</em>

<p>

Cluster ID for nats streaming, if it’s missing, treat it as NATS server

</p>

</td>

</tr>

<tr>

<td>

<code>auth</code></br> <em>
<a href="#argoproj.io/v1alpha1.AuthStrategy"> AuthStrategy </a> </em>

</td>

<td>

<em>(Optional)</em>

<p>

Auth strategy, default to AuthStrategyNone

</p>

</td>

</tr>

<tr>

<td>

<code>accessSecret</code></br> <em>
<a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.13/#secretkeyselector-v1-core">
Kubernetes core/v1.SecretKeySelector </a> </em>

</td>

<td>

<em>(Optional)</em>

<p>

Secret for auth

</p>

</td>

</tr>

</tbody>

</table>

<h3 id="argoproj.io/v1alpha1.NativeStrategy">

NativeStrategy

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.NATSBus">NATSBus</a>)

</p>

<p>

<p>

NativeStrategy indicates to install a native NATS service

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>size</code></br> <em> int </em>

</td>

<td>

<p>

Size is the NATS StatefulSet size

</p>

</td>

</tr>

<tr>

<td>

<code>auth</code></br> <em>
<a href="#argoproj.io/v1alpha1.AuthStrategy"> AuthStrategy </a> </em>

</td>

<td>

</td>

</tr>

<tr>

<td>

<code>antiAffinity</code></br> <em> bool </em>

</td>

<td>

</td>

</tr>

<tr>

<td>

<code>persistence</code></br> <em>
<a href="#argoproj.io/v1alpha1.PersistenceStrategy"> PersistenceStrategy
</a> </em>

</td>

<td>

<em>(Optional)</em>

</td>

</tr>

</tbody>

</table>

<h3 id="argoproj.io/v1alpha1.PersistenceStrategy">

PersistenceStrategy

</h3>

<p>

(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.NativeStrategy">NativeStrategy</a>)

</p>

<p>

<p>

PersistenceStrategy defines the strategy of persistence

</p>

</p>

<table>

<thead>

<tr>

<th>

Field

</th>

<th>

Description

</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<code>storageClassName</code></br> <em> string </em>

</td>

<td>

<em>(Optional)</em>

<p>

Name of the StorageClass required by the claim. More info:
<a href="https://kubernetes.io/docs/concepts/storage/persistent-volumes#class-1">https://kubernetes.io/docs/concepts/storage/persistent-volumes\#class-1</a>

</p>

</td>

</tr>

<tr>

<td>

<code>accessMode</code></br> <em>
<a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.13/#persistentvolumeaccessmode-v1-core">
Kubernetes core/v1.PersistentVolumeAccessMode </a> </em>

</td>

<td>

<em>(Optional)</em>

<p>

Available access modes such as ReadWriteOnce, ReadWriteMany
<a href="https://kubernetes.io/docs/concepts/storage/persistent-volumes/#access-modes">https://kubernetes.io/docs/concepts/storage/persistent-volumes/\#access-modes</a>

</p>

</td>

</tr>

<tr>

<td>

<code>size</code></br> <em>
k8s.io/apimachinery/pkg/api/resource.Quantity </em>

</td>

<td>

<p>

Volume size, e.g. 10Gi

</p>

</td>

</tr>

</tbody>

</table>

<hr/>

<p>

<em> Generated with <code>gen-crd-api-reference-docs</code>. </em>

</p>
