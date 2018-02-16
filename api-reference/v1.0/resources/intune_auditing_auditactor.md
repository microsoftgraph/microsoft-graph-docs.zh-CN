# <a name="auditactor-resource-type"></a><span data-ttu-id="09800-101">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="09800-101">auditActor resource type</span></span>

> <span data-ttu-id="09800-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="09800-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09800-103">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="09800-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="09800-104">属性</span><span class="sxs-lookup"><span data-stu-id="09800-104">Properties</span></span>
|<span data-ttu-id="09800-105">属性</span><span class="sxs-lookup"><span data-stu-id="09800-105">Property</span></span>|<span data-ttu-id="09800-106">类型</span><span class="sxs-lookup"><span data-stu-id="09800-106">Type</span></span>|<span data-ttu-id="09800-107">说明</span><span class="sxs-lookup"><span data-stu-id="09800-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09800-108">类型</span><span class="sxs-lookup"><span data-stu-id="09800-108">type</span></span>|<span data-ttu-id="09800-109">String</span><span class="sxs-lookup"><span data-stu-id="09800-109">String</span></span>|<span data-ttu-id="09800-110">主角类型。</span><span class="sxs-lookup"><span data-stu-id="09800-110">Actor Type.</span></span>|
|<span data-ttu-id="09800-111">权限</span><span class="sxs-lookup"><span data-stu-id="09800-111">permissions</span></span>|<span data-ttu-id="09800-112">String collection</span><span class="sxs-lookup"><span data-stu-id="09800-112">String collection</span></span>|<span data-ttu-id="09800-113">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="09800-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="09800-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="09800-114">userPermissions</span></span>|<span data-ttu-id="09800-115">String collection</span><span class="sxs-lookup"><span data-stu-id="09800-115">String collection</span></span>|<span data-ttu-id="09800-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="09800-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="09800-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="09800-117">applicationId</span></span>|<span data-ttu-id="09800-118">String</span><span class="sxs-lookup"><span data-stu-id="09800-118">String</span></span>|<span data-ttu-id="09800-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="09800-119">AAD Application Id.</span></span>|
|<span data-ttu-id="09800-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="09800-120">applicationDisplayName</span></span>|<span data-ttu-id="09800-121">String</span><span class="sxs-lookup"><span data-stu-id="09800-121">String</span></span>|<span data-ttu-id="09800-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="09800-122">Name of the Application.</span></span>|
|<span data-ttu-id="09800-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09800-123">userPrincipalName</span></span>|<span data-ttu-id="09800-124">String</span><span class="sxs-lookup"><span data-stu-id="09800-124">String</span></span>|<span data-ttu-id="09800-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="09800-125">User principal name (UPN)</span></span>|
|<span data-ttu-id="09800-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="09800-126">servicePrincipalName</span></span>|<span data-ttu-id="09800-127">String</span><span class="sxs-lookup"><span data-stu-id="09800-127">String</span></span>|<span data-ttu-id="09800-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="09800-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="09800-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="09800-129">ipAddress</span></span>|<span data-ttu-id="09800-130">String</span><span class="sxs-lookup"><span data-stu-id="09800-130">String</span></span>|<span data-ttu-id="09800-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="09800-131">IPAddress.</span></span>|
|<span data-ttu-id="09800-132">userId</span><span class="sxs-lookup"><span data-stu-id="09800-132">userID</span></span>|<span data-ttu-id="09800-133">String</span><span class="sxs-lookup"><span data-stu-id="09800-133">String</span></span>|<span data-ttu-id="09800-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="09800-134">User ID</span></span>|

## <a name="relationships"></a><span data-ttu-id="09800-135">关系</span><span class="sxs-lookup"><span data-stu-id="09800-135">Relationships</span></span>
<span data-ttu-id="09800-136">无</span><span class="sxs-lookup"><span data-stu-id="09800-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09800-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09800-137">JSON Representation</span></span>
<span data-ttu-id="09800-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09800-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
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
}
```



