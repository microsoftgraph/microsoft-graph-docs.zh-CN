# <a name="auditevent-resource-type"></a><span data-ttu-id="679e0-101">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="679e0-101">auditEvent resource type</span></span>

> <span data-ttu-id="679e0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="679e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="679e0-103">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="679e0-103">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="679e0-104">方法</span><span class="sxs-lookup"><span data-stu-id="679e0-104">Methods</span></span>
|<span data-ttu-id="679e0-105">方法</span><span class="sxs-lookup"><span data-stu-id="679e0-105">Method</span></span>|<span data-ttu-id="679e0-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="679e0-106">Return Type</span></span>|<span data-ttu-id="679e0-107">说明</span><span class="sxs-lookup"><span data-stu-id="679e0-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="679e0-108">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="679e0-108">List auditEvents</span></span>](../api/intune_auditing_auditevent_list.md)|<span data-ttu-id="679e0-109">[auditEvent](../resources/intune_auditing_auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="679e0-109">[auditEvent](../resources/intune_auditing_auditevent.md) collection</span></span>|<span data-ttu-id="679e0-110">列出 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="679e0-110">List properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) objects.</span></span>|
|[<span data-ttu-id="679e0-111">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="679e0-111">Get auditEvent</span></span>](../api/intune_auditing_auditevent_get.md)|[<span data-ttu-id="679e0-112">auditEvent</span><span class="sxs-lookup"><span data-stu-id="679e0-112">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="679e0-113">读取 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="679e0-113">Read properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="679e0-114">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="679e0-114">Create auditEvent</span></span>](../api/intune_auditing_auditevent_create.md)|[<span data-ttu-id="679e0-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="679e0-115">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="679e0-116">创建新的 [auditEvent](../resources/intune_auditing_auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="679e0-116">Create a new [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="679e0-117">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="679e0-117">Delete auditEvent</span></span>](../api/intune_auditing_auditevent_delete.md)|<span data-ttu-id="679e0-118">无</span><span class="sxs-lookup"><span data-stu-id="679e0-118">None</span></span>|<span data-ttu-id="679e0-119">删除 [auditEvent](../resources/intune_auditing_auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="679e0-119">Deletes a [auditEvent](../resources/intune_auditing_auditevent.md).</span></span>|
|[<span data-ttu-id="679e0-120">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="679e0-120">Update auditEvent</span></span>](../api/intune_auditing_auditevent_update.md)|[<span data-ttu-id="679e0-121">auditEvent</span><span class="sxs-lookup"><span data-stu-id="679e0-121">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="679e0-122">更新 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="679e0-122">Update the properties of a [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="679e0-123">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="679e0-123">getAuditCategories function</span></span>](../api/intune_auditing_auditevent_getauditcategories.md)|<span data-ttu-id="679e0-124">String collection</span><span class="sxs-lookup"><span data-stu-id="679e0-124">String collection</span></span>|<span data-ttu-id="679e0-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="679e0-125">Not yet documented</span></span>|
|[<span data-ttu-id="679e0-126">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="679e0-126">getAuditActivityTypes function</span></span>](../api/intune_auditing_auditevent_getauditactivitytypes.md)|<span data-ttu-id="679e0-127">String collection</span><span class="sxs-lookup"><span data-stu-id="679e0-127">String collection</span></span>|<span data-ttu-id="679e0-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="679e0-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="679e0-129">属性</span><span class="sxs-lookup"><span data-stu-id="679e0-129">Properties</span></span>
|<span data-ttu-id="679e0-130">属性</span><span class="sxs-lookup"><span data-stu-id="679e0-130">Property</span></span>|<span data-ttu-id="679e0-131">类型</span><span class="sxs-lookup"><span data-stu-id="679e0-131">Type</span></span>|<span data-ttu-id="679e0-132">说明</span><span class="sxs-lookup"><span data-stu-id="679e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="679e0-133">id</span><span class="sxs-lookup"><span data-stu-id="679e0-133">id</span></span>|<span data-ttu-id="679e0-134">String</span><span class="sxs-lookup"><span data-stu-id="679e0-134">String</span></span>|<span data-ttu-id="679e0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="679e0-135">Key of the entity.</span></span>|
|<span data-ttu-id="679e0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="679e0-136">displayName</span></span>|<span data-ttu-id="679e0-137">String</span><span class="sxs-lookup"><span data-stu-id="679e0-137">String</span></span>|<span data-ttu-id="679e0-138">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="679e0-138">Event display name.</span></span>|
|<span data-ttu-id="679e0-139">componentName</span><span class="sxs-lookup"><span data-stu-id="679e0-139">componentName</span></span>|<span data-ttu-id="679e0-140">String</span><span class="sxs-lookup"><span data-stu-id="679e0-140">String</span></span>|<span data-ttu-id="679e0-141">组件名称。</span><span class="sxs-lookup"><span data-stu-id="679e0-141">Component name.</span></span>|
|<span data-ttu-id="679e0-142">actor</span><span class="sxs-lookup"><span data-stu-id="679e0-142">actor</span></span>|[<span data-ttu-id="679e0-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="679e0-143">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="679e0-144">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="679e0-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="679e0-145">activity</span><span class="sxs-lookup"><span data-stu-id="679e0-145">activity</span></span>|<span data-ttu-id="679e0-146">String</span><span class="sxs-lookup"><span data-stu-id="679e0-146">String</span></span>|<span data-ttu-id="679e0-147">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="679e0-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="679e0-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="679e0-148">activityDateTime</span></span>|<span data-ttu-id="679e0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="679e0-149">DateTimeOffset</span></span>|<span data-ttu-id="679e0-150">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="679e0-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="679e0-151">activityType</span><span class="sxs-lookup"><span data-stu-id="679e0-151">activityType</span></span>|<span data-ttu-id="679e0-152">String</span><span class="sxs-lookup"><span data-stu-id="679e0-152">String</span></span>|<span data-ttu-id="679e0-153">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="679e0-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="679e0-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="679e0-154">activityOperationType</span></span>|<span data-ttu-id="679e0-155">String</span><span class="sxs-lookup"><span data-stu-id="679e0-155">String</span></span>|<span data-ttu-id="679e0-156">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="679e0-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="679e0-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="679e0-157">activityResult</span></span>|<span data-ttu-id="679e0-158">String</span><span class="sxs-lookup"><span data-stu-id="679e0-158">String</span></span>|<span data-ttu-id="679e0-159">活动结果。</span><span class="sxs-lookup"><span data-stu-id="679e0-159">The result of the activity.</span></span>|
|<span data-ttu-id="679e0-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="679e0-160">correlationId</span></span>|<span data-ttu-id="679e0-161">Guid</span><span class="sxs-lookup"><span data-stu-id="679e0-161">Guid</span></span>|<span data-ttu-id="679e0-162">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="679e0-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="679e0-163">resources</span><span class="sxs-lookup"><span data-stu-id="679e0-163">resources</span></span>|<span data-ttu-id="679e0-164">[auditResource](../resources/intune_auditing_auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="679e0-164">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="679e0-165">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="679e0-165">Resources being modified.</span></span>|
|<span data-ttu-id="679e0-166">category</span><span class="sxs-lookup"><span data-stu-id="679e0-166">category</span></span>|<span data-ttu-id="679e0-167">String</span><span class="sxs-lookup"><span data-stu-id="679e0-167">String</span></span>|<span data-ttu-id="679e0-168">审核类别。</span><span class="sxs-lookup"><span data-stu-id="679e0-168">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="679e0-169">关系</span><span class="sxs-lookup"><span data-stu-id="679e0-169">Relationships</span></span>
<span data-ttu-id="679e0-170">无</span><span class="sxs-lookup"><span data-stu-id="679e0-170">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="679e0-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="679e0-171">JSON Representation</span></span>
<span data-ttu-id="679e0-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="679e0-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```



