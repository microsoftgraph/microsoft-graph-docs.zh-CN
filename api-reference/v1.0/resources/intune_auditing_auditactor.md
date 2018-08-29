# <a name="auditactor-resource-type"></a><span data-ttu-id="3556d-101">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="3556d-101">auditActor resource type</span></span>

> <span data-ttu-id="3556d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3556d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3556d-103">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="3556d-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="3556d-104">属性</span><span class="sxs-lookup"><span data-stu-id="3556d-104">Properties</span></span>
|<span data-ttu-id="3556d-105">属性</span><span class="sxs-lookup"><span data-stu-id="3556d-105">Property</span></span>|<span data-ttu-id="3556d-106">类型</span><span class="sxs-lookup"><span data-stu-id="3556d-106">Type</span></span>|<span data-ttu-id="3556d-107">说明</span><span class="sxs-lookup"><span data-stu-id="3556d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3556d-108">类型</span><span class="sxs-lookup"><span data-stu-id="3556d-108">type</span></span>|<span data-ttu-id="3556d-109">String</span><span class="sxs-lookup"><span data-stu-id="3556d-109">String</span></span>|<span data-ttu-id="3556d-110">主角类型。</span><span class="sxs-lookup"><span data-stu-id="3556d-110">Actor Type.</span></span>|
|<span data-ttu-id="3556d-111">userPermissions</span><span class="sxs-lookup"><span data-stu-id="3556d-111">userPermissions</span></span>|<span data-ttu-id="3556d-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="3556d-112">String collection</span></span>|<span data-ttu-id="3556d-113">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="3556d-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="3556d-114">applicationId</span><span class="sxs-lookup"><span data-stu-id="3556d-114">applicationId</span></span>|<span data-ttu-id="3556d-115">String</span><span class="sxs-lookup"><span data-stu-id="3556d-115">String</span></span>|<span data-ttu-id="3556d-116">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="3556d-116">AAD Application Id.</span></span>|
|<span data-ttu-id="3556d-117">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="3556d-117">applicationDisplayName</span></span>|<span data-ttu-id="3556d-118">String</span><span class="sxs-lookup"><span data-stu-id="3556d-118">String</span></span>|<span data-ttu-id="3556d-119">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="3556d-119">Name of the Application.</span></span>|
|<span data-ttu-id="3556d-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3556d-120">userPrincipalName</span></span>|<span data-ttu-id="3556d-121">String</span><span class="sxs-lookup"><span data-stu-id="3556d-121">String</span></span>|<span data-ttu-id="3556d-122">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="3556d-122">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="3556d-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="3556d-123">servicePrincipalName</span></span>|<span data-ttu-id="3556d-124">String</span><span class="sxs-lookup"><span data-stu-id="3556d-124">String</span></span>|<span data-ttu-id="3556d-125">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="3556d-125">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="3556d-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3556d-126">ipAddress</span></span>|<span data-ttu-id="3556d-127">String</span><span class="sxs-lookup"><span data-stu-id="3556d-127">String</span></span>|<span data-ttu-id="3556d-128">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="3556d-128">IPAddress.</span></span>|
|<span data-ttu-id="3556d-129">userId</span><span class="sxs-lookup"><span data-stu-id="3556d-129">userId</span></span>|<span data-ttu-id="3556d-130">String</span><span class="sxs-lookup"><span data-stu-id="3556d-130">String</span></span>|<span data-ttu-id="3556d-131">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="3556d-131">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3556d-132">关系</span><span class="sxs-lookup"><span data-stu-id="3556d-132">Relationships</span></span>
<span data-ttu-id="3556d-133">无</span><span class="sxs-lookup"><span data-stu-id="3556d-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3556d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3556d-134">JSON Representation</span></span>
<span data-ttu-id="3556d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3556d-135">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
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
}
```



