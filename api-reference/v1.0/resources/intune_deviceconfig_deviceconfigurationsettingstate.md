# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="9c165-101">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c165-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="9c165-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9c165-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c165-103">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="9c165-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="9c165-104">属性</span><span class="sxs-lookup"><span data-stu-id="9c165-104">Properties</span></span>
|<span data-ttu-id="9c165-105">属性</span><span class="sxs-lookup"><span data-stu-id="9c165-105">Property</span></span>|<span data-ttu-id="9c165-106">类型</span><span class="sxs-lookup"><span data-stu-id="9c165-106">Type</span></span>|<span data-ttu-id="9c165-107">说明</span><span class="sxs-lookup"><span data-stu-id="9c165-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c165-108">设置</span><span class="sxs-lookup"><span data-stu-id="9c165-108">setting</span></span>|<span data-ttu-id="9c165-109">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-109">String</span></span>|<span data-ttu-id="9c165-110">报告的设置</span><span class="sxs-lookup"><span data-stu-id="9c165-110">The setting that is being reported</span></span>|
|<span data-ttu-id="9c165-111">settingName</span><span class="sxs-lookup"><span data-stu-id="9c165-111">settingName</span></span>|<span data-ttu-id="9c165-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-112">String</span></span>|<span data-ttu-id="9c165-113">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="9c165-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="9c165-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c165-114">instanceDisplayName</span></span>|<span data-ttu-id="9c165-115">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-115">String</span></span>|<span data-ttu-id="9c165-116">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="9c165-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="9c165-117">状态</span><span class="sxs-lookup"><span data-stu-id="9c165-117">state</span></span>|[<span data-ttu-id="9c165-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9c165-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="9c165-p101">设置的合规性状态。可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="9c165-p101">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="9c165-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="9c165-121">errorCode</span></span>|<span data-ttu-id="9c165-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9c165-122">Int64</span></span>|<span data-ttu-id="9c165-123">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="9c165-123">Error code for the setting</span></span>|
|<span data-ttu-id="9c165-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="9c165-124">errorDescription</span></span>|<span data-ttu-id="9c165-125">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-125">String</span></span>|<span data-ttu-id="9c165-126">错误说明</span><span class="sxs-lookup"><span data-stu-id="9c165-126">Error description</span></span>|
|<span data-ttu-id="9c165-127">userId</span><span class="sxs-lookup"><span data-stu-id="9c165-127">userId</span></span>|<span data-ttu-id="9c165-128">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-128">String</span></span>|<span data-ttu-id="9c165-129">UserId</span><span class="sxs-lookup"><span data-stu-id="9c165-129">UserId</span></span>|
|<span data-ttu-id="9c165-130">userName</span><span class="sxs-lookup"><span data-stu-id="9c165-130">userName</span></span>|<span data-ttu-id="9c165-131">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-131">String</span></span>|<span data-ttu-id="9c165-132">UserName</span><span class="sxs-lookup"><span data-stu-id="9c165-132">UserName</span></span>|
|<span data-ttu-id="9c165-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="9c165-133">userEmail</span></span>|<span data-ttu-id="9c165-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-134">String</span></span>|<span data-ttu-id="9c165-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="9c165-135">UserEmail</span></span>|
|<span data-ttu-id="9c165-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c165-136">userPrincipalName</span></span>|<span data-ttu-id="9c165-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-137">String</span></span>|<span data-ttu-id="9c165-138">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="9c165-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="9c165-139">来源</span><span class="sxs-lookup"><span data-stu-id="9c165-139">sources</span></span>|<span data-ttu-id="9c165-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c165-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="9c165-141">参与策略</span><span class="sxs-lookup"><span data-stu-id="9c165-141">Contributing policies</span></span>|
|<span data-ttu-id="9c165-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="9c165-142">currentValue</span></span>|<span data-ttu-id="9c165-143">字符串</span><span class="sxs-lookup"><span data-stu-id="9c165-143">String</span></span>|<span data-ttu-id="9c165-144">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="9c165-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c165-145">关系</span><span class="sxs-lookup"><span data-stu-id="9c165-145">Relationships</span></span>
<span data-ttu-id="9c165-146">无</span><span class="sxs-lookup"><span data-stu-id="9c165-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c165-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c165-147">JSON Representation</span></span>
<span data-ttu-id="9c165-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c165-148">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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








