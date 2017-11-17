# <a name="device-resource-type"></a><span data-ttu-id="b923b-101">设备资源类型</span><span class="sxs-lookup"><span data-stu-id="b923b-101">device resource type</span></span>

<span data-ttu-id="b923b-p101">表示在组织中注册的设备。也可以在云中使用设备注册服务或通过 Intune 创建设备。条件访问策略使用它们进行多重身份验证。这些设备范围很广，从台式机、笔记本电脑到手机和平板电脑均包括在内。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="b923b-p101">Represents a device registered in the organization. Devices can also be created in the cloud using the Device Registration Service or by Intune. They're used by conditional access policies for multi-factor authentication. These devices can range from desktop and laptop machines to phones and tablets. Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="b923b-107">通过该资源可以使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b923b-107">This resource lets you add your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>


## <a name="methods"></a><span data-ttu-id="b923b-108">方法</span><span class="sxs-lookup"><span data-stu-id="b923b-108">Methods</span></span>

| <span data-ttu-id="b923b-109">方法</span><span class="sxs-lookup"><span data-stu-id="b923b-109">Method</span></span>       | <span data-ttu-id="b923b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b923b-110">Return Type</span></span>  |<span data-ttu-id="b923b-111">说明</span><span class="sxs-lookup"><span data-stu-id="b923b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b923b-112">创建设备</span><span class="sxs-lookup"><span data-stu-id="b923b-112">Create device</span></span>](../api/device_post_devices.md) | [<span data-ttu-id="b923b-113">设备</span><span class="sxs-lookup"><span data-stu-id="b923b-113">device</span></span>](device.md) |<span data-ttu-id="b923b-114">在目录中新建注册设备。</span><span class="sxs-lookup"><span data-stu-id="b923b-114">Create a new registered device in the directory.</span></span>|
|[<span data-ttu-id="b923b-115">获取设备</span><span class="sxs-lookup"><span data-stu-id="b923b-115">Get device</span></span>](../api/device_get.md) | [<span data-ttu-id="b923b-116">设备</span><span class="sxs-lookup"><span data-stu-id="b923b-116">device</span></span>](device.md) |<span data-ttu-id="b923b-117">读取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b923b-117">Read properties and relationships of a device object.</span></span>|
|[<span data-ttu-id="b923b-118">列出设备</span><span class="sxs-lookup"><span data-stu-id="b923b-118">List devices</span></span>](../api/device_list.md) | <span data-ttu-id="b923b-119">[设备](device.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b923b-119">[device](device.md) collection</span></span>| <span data-ttu-id="b923b-120">检索目录中的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="b923b-120">Retrieve a list of devices registered in the directory.</span></span> |
|[<span data-ttu-id="b923b-121">更新设备</span><span class="sxs-lookup"><span data-stu-id="b923b-121">Update device</span></span>](../api/device_update.md) | [<span data-ttu-id="b923b-122">设备</span><span class="sxs-lookup"><span data-stu-id="b923b-122">device</span></span>](device.md) |<span data-ttu-id="b923b-123">更新 device 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b923b-123">Update the properties of a device object.</span></span> |
|[<span data-ttu-id="b923b-124">删除设备</span><span class="sxs-lookup"><span data-stu-id="b923b-124">Delete device</span></span>](../api/device_delete.md) | <span data-ttu-id="b923b-125">无</span><span class="sxs-lookup"><span data-stu-id="b923b-125">None</span></span> |<span data-ttu-id="b923b-126">删除 device 对象。</span><span class="sxs-lookup"><span data-stu-id="b923b-126">Delete a device object.</span></span> |
|[<span data-ttu-id="b923b-127">创建 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="b923b-127">Create registeredOwner</span></span>](../api/device_post_registeredowners.md) |[<span data-ttu-id="b923b-128">directoryObject</span><span class="sxs-lookup"><span data-stu-id="b923b-128">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="b923b-129">通过发布到 registeredOwners 导航属性，将用户添加为该设备的新所有者。</span><span class="sxs-lookup"><span data-stu-id="b923b-129">Add a user as a new owner of the device by posting to the registeredOwners navigation property.</span></span>|
|[<span data-ttu-id="b923b-130">列出 registeredOwners</span><span class="sxs-lookup"><span data-stu-id="b923b-130">List registeredOwners</span></span>](../api/device_list_registeredowners.md) |<span data-ttu-id="b923b-131">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b923b-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b923b-132">从 registeredOwners 导航属性中获取身份为设备的注册所有者的用户。</span><span class="sxs-lookup"><span data-stu-id="b923b-132">Get the users that are registered owners of the device from the registeredOwners navigation property.</span></span>|
|[<span data-ttu-id="b923b-133">创建 registeredUser</span><span class="sxs-lookup"><span data-stu-id="b923b-133">Create registeredUser</span></span>](../api/device_post_registeredusers.md) |[<span data-ttu-id="b923b-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="b923b-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="b923b-135">通过发布到 registeredUsers 导航属性，为该设备添加新注册用户。</span><span class="sxs-lookup"><span data-stu-id="b923b-135">Add a registered user for the device by posting to the registeredUsers navigation property.</span></span>|
|[<span data-ttu-id="b923b-136">列出 registeredUsers</span><span class="sxs-lookup"><span data-stu-id="b923b-136">List registeredUsers</span></span>](../api/device_list_registeredusers.md) |<span data-ttu-id="b923b-137">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b923b-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b923b-138">从 registeredUsers 导航属性获取设备的注册用户。</span><span class="sxs-lookup"><span data-stu-id="b923b-138">Get the registered users of the device from the registeredUsers navigation property.</span></span>|
|<span data-ttu-id="b923b-139">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="b923b-139">**Open extensions**</span></span>| | |
|[<span data-ttu-id="b923b-140">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="b923b-140">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="b923b-141">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b923b-141">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="b923b-142">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="b923b-142">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="b923b-143">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="b923b-143">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="b923b-144">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b923b-144">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="b923b-145">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="b923b-145">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="b923b-146">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="b923b-146">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="b923b-147">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="b923b-147">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="b923b-148">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="b923b-148">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="b923b-149">属性</span><span class="sxs-lookup"><span data-stu-id="b923b-149">Properties</span></span>
| <span data-ttu-id="b923b-150">属性</span><span class="sxs-lookup"><span data-stu-id="b923b-150">Property</span></span>     | <span data-ttu-id="b923b-151">类型</span><span class="sxs-lookup"><span data-stu-id="b923b-151">Type</span></span>   |<span data-ttu-id="b923b-152">说明</span><span class="sxs-lookup"><span data-stu-id="b923b-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b923b-153">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b923b-153">accountEnabled</span></span>|<span data-ttu-id="b923b-154">布尔</span><span class="sxs-lookup"><span data-stu-id="b923b-154">Boolean</span></span>| <span data-ttu-id="b923b-p102">启用帐户时为 **true**，否则为 **false**。必需。</span><span class="sxs-lookup"><span data-stu-id="b923b-p102">**true** if the account is enabled; otherwise, **false**. Required.</span></span>|
|<span data-ttu-id="b923b-157">alternativeSecurityIds</span><span class="sxs-lookup"><span data-stu-id="b923b-157">alternativeSecurityIds</span></span>|<span data-ttu-id="b923b-158">[alternativeSecurityId](alternativesecurityid.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b923b-158">[alternativeSecurityId](alternativesecurityid.md) collection</span></span>| <span data-ttu-id="b923b-p103">需要多值属性筛选器表达式的**任意**运算符。不可为 NULL。必需。</span><span class="sxs-lookup"><span data-stu-id="b923b-p103">The **any** operator is required for filter expressions on multi-valued properties. Not nullable. Required.</span></span> |
|<span data-ttu-id="b923b-162">approximateLastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="b923b-162">approximateLastSignInDateTime</span></span>|<span data-ttu-id="b923b-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b923b-163">DateTimeOffset</span></span>| <span data-ttu-id="b923b-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b923b-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b923b-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="b923b-166">deviceId</span></span>|<span data-ttu-id="b923b-167">Guid</span><span class="sxs-lookup"><span data-stu-id="b923b-167">Guid</span></span>| <span data-ttu-id="b923b-p105">唯一客户端指定 GUID 以表示该设备。必需。</span><span class="sxs-lookup"><span data-stu-id="b923b-p105">Unique client specified GUID to represent the device. Required.</span></span> |
|<span data-ttu-id="b923b-170">deviceMetadata</span><span class="sxs-lookup"><span data-stu-id="b923b-170">deviceMetadata</span></span>|<span data-ttu-id="b923b-171">String</span><span class="sxs-lookup"><span data-stu-id="b923b-171">String</span></span>|    |
|<span data-ttu-id="b923b-172">deviceVersion</span><span class="sxs-lookup"><span data-stu-id="b923b-172">deviceVersion</span></span>|<span data-ttu-id="b923b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b923b-173">Int32</span></span>|            |
|<span data-ttu-id="b923b-174">displayName</span><span class="sxs-lookup"><span data-stu-id="b923b-174">displayName</span></span>|<span data-ttu-id="b923b-175">String</span><span class="sxs-lookup"><span data-stu-id="b923b-175">String</span></span>|<span data-ttu-id="b923b-p106">设备显示名称。必需。</span><span class="sxs-lookup"><span data-stu-id="b923b-p106">The display name for the device. Required.</span></span> |
|<span data-ttu-id="b923b-178">id</span><span class="sxs-lookup"><span data-stu-id="b923b-178">id</span></span>|<span data-ttu-id="b923b-179">String</span><span class="sxs-lookup"><span data-stu-id="b923b-179">String</span></span>|<span data-ttu-id="b923b-p107">设备唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL。只读。</span><span class="sxs-lookup"><span data-stu-id="b923b-p107">The unique identifier for the device. Inherited from [directoryObject](directoryobject.md). Key, Not nullable. Read-only.</span></span>|
|<span data-ttu-id="b923b-184">isCompliant</span><span class="sxs-lookup"><span data-stu-id="b923b-184">isCompliant</span></span>|<span data-ttu-id="b923b-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b923b-185">Boolean</span></span>|<span data-ttu-id="b923b-186">如果设备符合移动设备管理 (MDM) 策略，则为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="b923b-186">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span>|
|<span data-ttu-id="b923b-187">isManaged</span><span class="sxs-lookup"><span data-stu-id="b923b-187">isManaged</span></span>|<span data-ttu-id="b923b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b923b-188">Boolean</span></span>|<span data-ttu-id="b923b-189">如果用移动设备管理 (MDM) 应用（例如 Intune）管理设备，则为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="b923b-189">**true** if the device is managed by a Mobile Device Management (MDM) app such as Intune; otherwise, **false**.</span></span>|
|<span data-ttu-id="b923b-190">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b923b-190">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="b923b-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b923b-191">DateTimeOffset</span></span>|<span data-ttu-id="b923b-p108">对象最后一次与本地目录同步的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b923b-p108">The last time at which the object was synced with the on-premises directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b923b-194">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="b923b-194">onPremisesSyncEnabled</span></span>|<span data-ttu-id="b923b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b923b-195">Boolean</span></span>|<span data-ttu-id="b923b-196">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **NULL**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="b923b-196">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="b923b-197">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b923b-197">operatingSystem</span></span>|<span data-ttu-id="b923b-198">String</span><span class="sxs-lookup"><span data-stu-id="b923b-198">String</span></span>|<span data-ttu-id="b923b-p109">设备上操作系统的类型。必需。</span><span class="sxs-lookup"><span data-stu-id="b923b-p109">The type of operating system on the device. Required.</span></span> |
|<span data-ttu-id="b923b-201">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="b923b-201">operatingSystemVersion</span></span>|<span data-ttu-id="b923b-202">String</span><span class="sxs-lookup"><span data-stu-id="b923b-202">String</span></span>|<span data-ttu-id="b923b-p110">设备上操作系统的版本。必需。</span><span class="sxs-lookup"><span data-stu-id="b923b-p110">The version of the operating system on the device. Required.</span></span> |
|<span data-ttu-id="b923b-205">physicalIds</span><span class="sxs-lookup"><span data-stu-id="b923b-205">physicalIds</span></span>|<span data-ttu-id="b923b-206">String collection</span><span class="sxs-lookup"><span data-stu-id="b923b-206">String collection</span></span>| <span data-ttu-id="b923b-207">不可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b923b-207">Not nullable.</span></span>            |
|<span data-ttu-id="b923b-208">trustType</span><span class="sxs-lookup"><span data-stu-id="b923b-208">trustType</span></span>|<span data-ttu-id="b923b-209">String</span><span class="sxs-lookup"><span data-stu-id="b923b-209">String</span></span>|    ||

## <a name="relationships"></a><span data-ttu-id="b923b-210">关系</span><span class="sxs-lookup"><span data-stu-id="b923b-210">Relationships</span></span>
| <span data-ttu-id="b923b-211">关系</span><span class="sxs-lookup"><span data-stu-id="b923b-211">Relationship</span></span> | <span data-ttu-id="b923b-212">类型</span><span class="sxs-lookup"><span data-stu-id="b923b-212">Type</span></span>   |<span data-ttu-id="b923b-213">说明</span><span class="sxs-lookup"><span data-stu-id="b923b-213">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b923b-214">extensions</span><span class="sxs-lookup"><span data-stu-id="b923b-214">extensions</span></span>|<span data-ttu-id="b923b-215">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="b923b-215">[extension](extension.md) collection</span></span>|<span data-ttu-id="b923b-p111">为设备定义的开放扩展集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b923b-p111">The collection of open extensions defined for the device. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b923b-219">registeredOwners</span><span class="sxs-lookup"><span data-stu-id="b923b-219">registeredOwners</span></span>|<span data-ttu-id="b923b-220">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b923b-220">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="b923b-p112">是设备注册所有者的用户。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b923b-p112">Users that are registered owners of the device. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b923b-224">registeredUsers</span><span class="sxs-lookup"><span data-stu-id="b923b-224">registeredUsers</span></span>|<span data-ttu-id="b923b-225">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b923b-225">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="b923b-p113">身份为设备注册用户的用户。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b923b-p113">Users that are registered users of the device. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b923b-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b923b-229">JSON representation</span></span>

<span data-ttu-id="b923b-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b923b-230">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="b923b-231">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b923b-231">See also</span></span>

- [<span data-ttu-id="b923b-232">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b923b-232">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b923b-233">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b923b-233">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="b923b-234">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b923b-234">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
