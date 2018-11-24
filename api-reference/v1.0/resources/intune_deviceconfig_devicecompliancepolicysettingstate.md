# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="828a3-101">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="828a3-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="828a3-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="828a3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="828a3-103">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="828a3-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="828a3-104">属性</span><span class="sxs-lookup"><span data-stu-id="828a3-104">Properties</span></span>
|<span data-ttu-id="828a3-105">属性</span><span class="sxs-lookup"><span data-stu-id="828a3-105">Property</span></span>|<span data-ttu-id="828a3-106">类型</span><span class="sxs-lookup"><span data-stu-id="828a3-106">Type</span></span>|<span data-ttu-id="828a3-107">说明</span><span class="sxs-lookup"><span data-stu-id="828a3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="828a3-108">setting</span><span class="sxs-lookup"><span data-stu-id="828a3-108">setting</span></span>|<span data-ttu-id="828a3-109">String</span><span class="sxs-lookup"><span data-stu-id="828a3-109">String</span></span>|<span data-ttu-id="828a3-110">报告的设置</span><span class="sxs-lookup"><span data-stu-id="828a3-110">The setting that is being reported</span></span>|
|<span data-ttu-id="828a3-111">settingName</span><span class="sxs-lookup"><span data-stu-id="828a3-111">settingName</span></span>|<span data-ttu-id="828a3-112">String</span><span class="sxs-lookup"><span data-stu-id="828a3-112">String</span></span>|<span data-ttu-id="828a3-113">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="828a3-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="828a3-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="828a3-114">instanceDisplayName</span></span>|<span data-ttu-id="828a3-115">String</span><span class="sxs-lookup"><span data-stu-id="828a3-115">String</span></span>|<span data-ttu-id="828a3-116">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="828a3-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="828a3-117">state</span><span class="sxs-lookup"><span data-stu-id="828a3-117">state</span></span>|[<span data-ttu-id="828a3-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="828a3-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="828a3-119">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="828a3-119">The compliance state of the setting.</span></span> <span data-ttu-id="828a3-120">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="828a3-120">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="828a3-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="828a3-121">errorCode</span></span>|<span data-ttu-id="828a3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="828a3-122">Int64</span></span>|<span data-ttu-id="828a3-123">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="828a3-123">Error code for the setting</span></span>|
|<span data-ttu-id="828a3-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="828a3-124">errorDescription</span></span>|<span data-ttu-id="828a3-125">String</span><span class="sxs-lookup"><span data-stu-id="828a3-125">String</span></span>|<span data-ttu-id="828a3-126">错误说明</span><span class="sxs-lookup"><span data-stu-id="828a3-126">Error description</span></span>|
|<span data-ttu-id="828a3-127">userId</span><span class="sxs-lookup"><span data-stu-id="828a3-127">userId</span></span>|<span data-ttu-id="828a3-128">String</span><span class="sxs-lookup"><span data-stu-id="828a3-128">String</span></span>|<span data-ttu-id="828a3-129">UserId</span><span class="sxs-lookup"><span data-stu-id="828a3-129">UserId</span></span>|
|<span data-ttu-id="828a3-130">userName</span><span class="sxs-lookup"><span data-stu-id="828a3-130">userName</span></span>|<span data-ttu-id="828a3-131">String</span><span class="sxs-lookup"><span data-stu-id="828a3-131">String</span></span>|<span data-ttu-id="828a3-132">UserName</span><span class="sxs-lookup"><span data-stu-id="828a3-132">UserName</span></span>|
|<span data-ttu-id="828a3-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="828a3-133">userEmail</span></span>|<span data-ttu-id="828a3-134">String</span><span class="sxs-lookup"><span data-stu-id="828a3-134">String</span></span>|<span data-ttu-id="828a3-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="828a3-135">UserEmail</span></span>|
|<span data-ttu-id="828a3-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="828a3-136">userPrincipalName</span></span>|<span data-ttu-id="828a3-137">String</span><span class="sxs-lookup"><span data-stu-id="828a3-137">String</span></span>|<span data-ttu-id="828a3-138">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="828a3-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="828a3-139">sources</span><span class="sxs-lookup"><span data-stu-id="828a3-139">sources</span></span>|<span data-ttu-id="828a3-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="828a3-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="828a3-141">参与策略</span><span class="sxs-lookup"><span data-stu-id="828a3-141">Contributing policies</span></span>|
|<span data-ttu-id="828a3-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="828a3-142">currentValue</span></span>|<span data-ttu-id="828a3-143">String</span><span class="sxs-lookup"><span data-stu-id="828a3-143">String</span></span>|<span data-ttu-id="828a3-144">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="828a3-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="828a3-145">关系</span><span class="sxs-lookup"><span data-stu-id="828a3-145">Relationships</span></span>
<span data-ttu-id="828a3-146">无</span><span class="sxs-lookup"><span data-stu-id="828a3-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="828a3-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="828a3-147">JSON Representation</span></span>
<span data-ttu-id="828a3-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="828a3-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



