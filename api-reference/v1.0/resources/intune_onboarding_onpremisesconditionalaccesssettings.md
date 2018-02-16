# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="89a74-101">onPremisesConditionalAccessSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="89a74-101">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="89a74-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89a74-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89a74-103">表示租户的 Exchange 本地条件访问设置的单例实体。</span><span class="sxs-lookup"><span data-stu-id="89a74-103">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="89a74-104">方法</span><span class="sxs-lookup"><span data-stu-id="89a74-104">Methods</span></span>
|<span data-ttu-id="89a74-105">方法</span><span class="sxs-lookup"><span data-stu-id="89a74-105">Method</span></span>|<span data-ttu-id="89a74-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="89a74-106">Return Type</span></span>|<span data-ttu-id="89a74-107">说明</span><span class="sxs-lookup"><span data-stu-id="89a74-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89a74-108">获取 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="89a74-108">Get onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[<span data-ttu-id="89a74-109">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="89a74-109">onpremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="89a74-110">读取 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89a74-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="89a74-111">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="89a74-111">Update onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[<span data-ttu-id="89a74-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="89a74-112">onpremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="89a74-113">更新 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89a74-113">Update the properties of a [calendar](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89a74-114">属性</span><span class="sxs-lookup"><span data-stu-id="89a74-114">Properties</span></span>
|<span data-ttu-id="89a74-115">属性</span><span class="sxs-lookup"><span data-stu-id="89a74-115">Property</span></span>|<span data-ttu-id="89a74-116">类型</span><span class="sxs-lookup"><span data-stu-id="89a74-116">Type</span></span>|<span data-ttu-id="89a74-117">说明</span><span class="sxs-lookup"><span data-stu-id="89a74-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a74-118">id</span><span class="sxs-lookup"><span data-stu-id="89a74-118">id</span></span>|<span data-ttu-id="89a74-119">String</span><span class="sxs-lookup"><span data-stu-id="89a74-119">String</span></span>|<span data-ttu-id="89a74-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89a74-120">Not yet documented</span></span>|
|<span data-ttu-id="89a74-121">已启用</span><span class="sxs-lookup"><span data-stu-id="89a74-121">enabled</span></span>|<span data-ttu-id="89a74-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="89a74-122">Boolean</span></span>|<span data-ttu-id="89a74-123">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="89a74-123">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="89a74-124">includedGroups</span><span class="sxs-lookup"><span data-stu-id="89a74-124">includedGroups</span></span>|<span data-ttu-id="89a74-125">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="89a74-125">Guid collection</span></span>|<span data-ttu-id="89a74-126">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="89a74-126">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="89a74-127">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="89a74-127">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="89a74-128">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="89a74-128">excludedGroups</span></span>|<span data-ttu-id="89a74-129">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="89a74-129">Guid collection</span></span>|<span data-ttu-id="89a74-130">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="89a74-130">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="89a74-131">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="89a74-131">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="89a74-132">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="89a74-132">overrideDefaultRule</span></span>|<span data-ttu-id="89a74-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="89a74-133">Boolean</span></span>|<span data-ttu-id="89a74-134">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="89a74-134">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89a74-135">关系</span><span class="sxs-lookup"><span data-stu-id="89a74-135">Relationships</span></span>
<span data-ttu-id="89a74-136">无</span><span class="sxs-lookup"><span data-stu-id="89a74-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89a74-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89a74-137">JSON Representation</span></span>
<span data-ttu-id="89a74-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89a74-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```



