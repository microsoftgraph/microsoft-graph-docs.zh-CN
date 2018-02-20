# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="85e77-101">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="85e77-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="85e77-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="85e77-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85e77-103">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="85e77-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="85e77-104">属性</span><span class="sxs-lookup"><span data-stu-id="85e77-104">Properties</span></span>
|<span data-ttu-id="85e77-105">属性</span><span class="sxs-lookup"><span data-stu-id="85e77-105">Property</span></span>|<span data-ttu-id="85e77-106">类型</span><span class="sxs-lookup"><span data-stu-id="85e77-106">Type</span></span>|<span data-ttu-id="85e77-107">说明</span><span class="sxs-lookup"><span data-stu-id="85e77-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e77-108">setting</span><span class="sxs-lookup"><span data-stu-id="85e77-108">setting</span></span>|<span data-ttu-id="85e77-109">String</span><span class="sxs-lookup"><span data-stu-id="85e77-109">String</span></span>|<span data-ttu-id="85e77-110">报告的设置</span><span class="sxs-lookup"><span data-stu-id="85e77-110">The setting that is being reported</span></span>|
|<span data-ttu-id="85e77-111">settingName</span><span class="sxs-lookup"><span data-stu-id="85e77-111">settingName</span></span>|<span data-ttu-id="85e77-112">String</span><span class="sxs-lookup"><span data-stu-id="85e77-112">String</span></span>|<span data-ttu-id="85e77-113">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="85e77-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="85e77-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="85e77-114">instanceDisplayName</span></span>|<span data-ttu-id="85e77-115">String</span><span class="sxs-lookup"><span data-stu-id="85e77-115">String</span></span>|<span data-ttu-id="85e77-116">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="85e77-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="85e77-117">state</span><span class="sxs-lookup"><span data-stu-id="85e77-117">state</span></span>|<span data-ttu-id="85e77-118">String</span><span class="sxs-lookup"><span data-stu-id="85e77-118">String</span></span>|<span data-ttu-id="85e77-119">设置的符合性状态 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="85e77-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="85e77-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="85e77-120">errorCode</span></span>|<span data-ttu-id="85e77-121">Int64</span><span class="sxs-lookup"><span data-stu-id="85e77-121">Int64</span></span>|<span data-ttu-id="85e77-122">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="85e77-122">Error code for the setting</span></span>|
|<span data-ttu-id="85e77-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="85e77-123">error_description</span></span>|<span data-ttu-id="85e77-124">String</span><span class="sxs-lookup"><span data-stu-id="85e77-124">String</span></span>|<span data-ttu-id="85e77-125">错误说明</span><span class="sxs-lookup"><span data-stu-id="85e77-125">Error Description</span></span>|
|<span data-ttu-id="85e77-126">userId</span><span class="sxs-lookup"><span data-stu-id="85e77-126">userID</span></span>|<span data-ttu-id="85e77-127">String</span><span class="sxs-lookup"><span data-stu-id="85e77-127">String</span></span>|<span data-ttu-id="85e77-128">UserId</span><span class="sxs-lookup"><span data-stu-id="85e77-128">UserId</span></span>|
|<span data-ttu-id="85e77-129">userName</span><span class="sxs-lookup"><span data-stu-id="85e77-129">UserName</span></span>|<span data-ttu-id="85e77-130">String</span><span class="sxs-lookup"><span data-stu-id="85e77-130">String</span></span>|<span data-ttu-id="85e77-131">UserName</span><span class="sxs-lookup"><span data-stu-id="85e77-131">UserName</span></span>|
|<span data-ttu-id="85e77-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="85e77-132">userEmail</span></span>|<span data-ttu-id="85e77-133">String</span><span class="sxs-lookup"><span data-stu-id="85e77-133">String</span></span>|<span data-ttu-id="85e77-134">UserEmail</span><span class="sxs-lookup"><span data-stu-id="85e77-134">UserEmail Element</span></span>|
|<span data-ttu-id="85e77-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85e77-135">userPrincipalName</span></span>|<span data-ttu-id="85e77-136">String</span><span class="sxs-lookup"><span data-stu-id="85e77-136">String</span></span>|<span data-ttu-id="85e77-137">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="85e77-137">userPrincipalName</span></span>|
|<span data-ttu-id="85e77-138">sources</span><span class="sxs-lookup"><span data-stu-id="85e77-138">Content sources</span></span>|<span data-ttu-id="85e77-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85e77-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="85e77-140">参与策略</span><span class="sxs-lookup"><span data-stu-id="85e77-140">Contributing policies</span></span>|
|<span data-ttu-id="85e77-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="85e77-141">currentValue</span></span>|<span data-ttu-id="85e77-142">String</span><span class="sxs-lookup"><span data-stu-id="85e77-142">String</span></span>|<span data-ttu-id="85e77-143">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="85e77-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="85e77-144">关系</span><span class="sxs-lookup"><span data-stu-id="85e77-144">Relationships</span></span>
<span data-ttu-id="85e77-145">无</span><span class="sxs-lookup"><span data-stu-id="85e77-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85e77-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85e77-146">JSON Representation</span></span>
<span data-ttu-id="85e77-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85e77-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



