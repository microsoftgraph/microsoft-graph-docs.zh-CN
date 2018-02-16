# <a name="auditevent-resource-type"></a><span data-ttu-id="108e3-101">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="108e3-101">auditEvent resource type</span></span>

> <span data-ttu-id="108e3-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="108e3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="108e3-103">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="108e3-103">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="108e3-104">方法</span><span class="sxs-lookup"><span data-stu-id="108e3-104">Methods</span></span>
|<span data-ttu-id="108e3-105">方法</span><span class="sxs-lookup"><span data-stu-id="108e3-105">Method</span></span>|<span data-ttu-id="108e3-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="108e3-106">Return Type</span></span>|<span data-ttu-id="108e3-107">说明</span><span class="sxs-lookup"><span data-stu-id="108e3-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="108e3-108">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="108e3-108">List auditEvents</span></span>](../api/intune_auditing_auditevent_list.md)|<span data-ttu-id="108e3-109">[auditEvent](../resources/intune_auditing_auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="108e3-109">[auditEvent](../resources/intune_auditing_auditevent.md) collection</span></span>|<span data-ttu-id="108e3-110">列出 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="108e3-110">List properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) objects.</span></span>|
|[<span data-ttu-id="108e3-111">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="108e3-111">Get auditEvent</span></span>](../api/intune_auditing_auditevent_get.md)|[<span data-ttu-id="108e3-112">auditEvent</span><span class="sxs-lookup"><span data-stu-id="108e3-112">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="108e3-113">读取 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="108e3-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="108e3-114">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="108e3-114">Create auditEvent</span></span>](../api/intune_auditing_auditevent_create.md)|[<span data-ttu-id="108e3-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="108e3-115">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="108e3-116">创建新的 [auditEvent](../resources/intune_auditing_auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="108e3-116">Create a new [plannerBucket](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="108e3-117">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="108e3-117">Delete auditEvent</span></span>](../api/intune_auditing_auditevent_delete.md)|<span data-ttu-id="108e3-118">无</span><span class="sxs-lookup"><span data-stu-id="108e3-118">None</span></span>|<span data-ttu-id="108e3-119">删除 [auditEvent](../resources/intune_auditing_auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="108e3-119">Deletes a [auditEvent](../resources/intune_auditing_auditevent.md).</span></span>|
|[<span data-ttu-id="108e3-120">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="108e3-120">Update auditEvent</span></span>](../api/intune_auditing_auditevent_update.md)|[<span data-ttu-id="108e3-121">auditEvent</span><span class="sxs-lookup"><span data-stu-id="108e3-121">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="108e3-122">更新 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="108e3-122">Update the properties of a [calendar](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="108e3-123">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="108e3-123">getAuditCategories function</span></span>](../api/intune_auditing_auditevent_getauditcategories.md)|<span data-ttu-id="108e3-124">String collection</span><span class="sxs-lookup"><span data-stu-id="108e3-124">String collection</span></span>|<span data-ttu-id="108e3-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="108e3-125">Not yet documented</span></span>|
|[<span data-ttu-id="108e3-126">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="108e3-126">getAuditActivityTypes function</span></span>](../api/intune_auditing_auditevent_getauditactivitytypes.md)|<span data-ttu-id="108e3-127">String collection</span><span class="sxs-lookup"><span data-stu-id="108e3-127">String collection</span></span>|<span data-ttu-id="108e3-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="108e3-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="108e3-129">属性</span><span class="sxs-lookup"><span data-stu-id="108e3-129">Properties</span></span>
|<span data-ttu-id="108e3-130">属性</span><span class="sxs-lookup"><span data-stu-id="108e3-130">Property</span></span>|<span data-ttu-id="108e3-131">类型</span><span class="sxs-lookup"><span data-stu-id="108e3-131">Type</span></span>|<span data-ttu-id="108e3-132">说明</span><span class="sxs-lookup"><span data-stu-id="108e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="108e3-133">id</span><span class="sxs-lookup"><span data-stu-id="108e3-133">id</span></span>|<span data-ttu-id="108e3-134">String</span><span class="sxs-lookup"><span data-stu-id="108e3-134">String</span></span>|<span data-ttu-id="108e3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="108e3-135">Key of the setting.</span></span>|
|<span data-ttu-id="108e3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="108e3-136">displayName</span></span>|<span data-ttu-id="108e3-137">String</span><span class="sxs-lookup"><span data-stu-id="108e3-137">String</span></span>|<span data-ttu-id="108e3-138">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="108e3-138">Event display name.</span></span>|
|<span data-ttu-id="108e3-139">componentName</span><span class="sxs-lookup"><span data-stu-id="108e3-139">--componentName</span></span>|<span data-ttu-id="108e3-140">String</span><span class="sxs-lookup"><span data-stu-id="108e3-140">String</span></span>|<span data-ttu-id="108e3-141">组件名称。</span><span class="sxs-lookup"><span data-stu-id="108e3-141">Component name.</span></span>|
|<span data-ttu-id="108e3-142">actor</span><span class="sxs-lookup"><span data-stu-id="108e3-142">actor</span></span>|[<span data-ttu-id="108e3-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="108e3-143">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="108e3-144">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="108e3-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="108e3-145">activity</span><span class="sxs-lookup"><span data-stu-id="108e3-145">activity</span></span>|<span data-ttu-id="108e3-146">String</span><span class="sxs-lookup"><span data-stu-id="108e3-146">String</span></span>|<span data-ttu-id="108e3-147">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="108e3-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="108e3-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="108e3-148">activityDateTime</span></span>|<span data-ttu-id="108e3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="108e3-149">DateTimeOffset</span></span>|<span data-ttu-id="108e3-150">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="108e3-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="108e3-151">activityType</span><span class="sxs-lookup"><span data-stu-id="108e3-151">activityType</span></span>|<span data-ttu-id="108e3-152">String</span><span class="sxs-lookup"><span data-stu-id="108e3-152">String</span></span>|<span data-ttu-id="108e3-153">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="108e3-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="108e3-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="108e3-154">activityOperationType</span></span>|<span data-ttu-id="108e3-155">String</span><span class="sxs-lookup"><span data-stu-id="108e3-155">String</span></span>|<span data-ttu-id="108e3-156">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="108e3-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="108e3-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="108e3-157">activityResult</span></span>|<span data-ttu-id="108e3-158">String</span><span class="sxs-lookup"><span data-stu-id="108e3-158">String</span></span>|<span data-ttu-id="108e3-159">活动结果。</span><span class="sxs-lookup"><span data-stu-id="108e3-159">The result of the submission.</span></span>|
|<span data-ttu-id="108e3-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="108e3-160">correlationId</span></span>|<span data-ttu-id="108e3-161">Guid</span><span class="sxs-lookup"><span data-stu-id="108e3-161">Guid</span></span>|<span data-ttu-id="108e3-162">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="108e3-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="108e3-163">resources</span><span class="sxs-lookup"><span data-stu-id="108e3-163">resources</span></span>|<span data-ttu-id="108e3-164">[auditResource](../resources/intune_auditing_auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="108e3-164">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="108e3-165">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="108e3-165">Resources being modified.</span></span>|
|<span data-ttu-id="108e3-166">category</span><span class="sxs-lookup"><span data-stu-id="108e3-166">category</span></span>|<span data-ttu-id="108e3-167">String</span><span class="sxs-lookup"><span data-stu-id="108e3-167">String</span></span>|<span data-ttu-id="108e3-168">审核类别。</span><span class="sxs-lookup"><span data-stu-id="108e3-168">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="108e3-169">关系</span><span class="sxs-lookup"><span data-stu-id="108e3-169">Relationships</span></span>
<span data-ttu-id="108e3-170">无</span><span class="sxs-lookup"><span data-stu-id="108e3-170">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="108e3-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="108e3-171">JSON Representation</span></span>
<span data-ttu-id="108e3-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="108e3-172">Here is a JSON representation of the resource.</span></span>
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
    "permissions": [
      "String"
    ],
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
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
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



