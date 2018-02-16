# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="cc20f-101">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc20f-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="cc20f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cc20f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc20f-103">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="cc20f-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="cc20f-104">属性</span><span class="sxs-lookup"><span data-stu-id="cc20f-104">Properties</span></span>
|<span data-ttu-id="cc20f-105">属性</span><span class="sxs-lookup"><span data-stu-id="cc20f-105">Property</span></span>|<span data-ttu-id="cc20f-106">类型</span><span class="sxs-lookup"><span data-stu-id="cc20f-106">Type</span></span>|<span data-ttu-id="cc20f-107">说明</span><span class="sxs-lookup"><span data-stu-id="cc20f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc20f-108">setting</span><span class="sxs-lookup"><span data-stu-id="cc20f-108">setting</span></span>|<span data-ttu-id="cc20f-109">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-109">String</span></span>|<span data-ttu-id="cc20f-110">报告的设置</span><span class="sxs-lookup"><span data-stu-id="cc20f-110">The setting that is being reported</span></span>|
|<span data-ttu-id="cc20f-111">settingName</span><span class="sxs-lookup"><span data-stu-id="cc20f-111">settingName</span></span>|<span data-ttu-id="cc20f-112">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-112">String</span></span>|<span data-ttu-id="cc20f-113">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="cc20f-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="cc20f-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cc20f-114">instanceDisplayName</span></span>|<span data-ttu-id="cc20f-115">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-115">String</span></span>|<span data-ttu-id="cc20f-116">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="cc20f-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="cc20f-117">state</span><span class="sxs-lookup"><span data-stu-id="cc20f-117">state</span></span>|<span data-ttu-id="cc20f-118">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-118">String</span></span>|<span data-ttu-id="cc20f-119">设置的符合性状态 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="cc20f-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="cc20f-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="cc20f-120">errorCode</span></span>|<span data-ttu-id="cc20f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="cc20f-121">Int64</span></span>|<span data-ttu-id="cc20f-122">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="cc20f-122">Error code for the setting</span></span>|
|<span data-ttu-id="cc20f-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="cc20f-123">error_description</span></span>|<span data-ttu-id="cc20f-124">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-124">String</span></span>|<span data-ttu-id="cc20f-125">错误说明</span><span class="sxs-lookup"><span data-stu-id="cc20f-125">Error Description</span></span>|
|<span data-ttu-id="cc20f-126">userId</span><span class="sxs-lookup"><span data-stu-id="cc20f-126">userID</span></span>|<span data-ttu-id="cc20f-127">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-127">String</span></span>|<span data-ttu-id="cc20f-128">UserId</span><span class="sxs-lookup"><span data-stu-id="cc20f-128">UserId</span></span>|
|<span data-ttu-id="cc20f-129">userName</span><span class="sxs-lookup"><span data-stu-id="cc20f-129">UserName</span></span>|<span data-ttu-id="cc20f-130">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-130">String</span></span>|<span data-ttu-id="cc20f-131">UserName</span><span class="sxs-lookup"><span data-stu-id="cc20f-131">UserName</span></span>|
|<span data-ttu-id="cc20f-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="cc20f-132">userEmail</span></span>|<span data-ttu-id="cc20f-133">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-133">String</span></span>|<span data-ttu-id="cc20f-134">UserEmail</span><span class="sxs-lookup"><span data-stu-id="cc20f-134">UserEmail Element</span></span>|
|<span data-ttu-id="cc20f-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cc20f-135">userPrincipalName</span></span>|<span data-ttu-id="cc20f-136">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-136">String</span></span>|<span data-ttu-id="cc20f-137">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="cc20f-137">userPrincipalName</span></span>|
|<span data-ttu-id="cc20f-138">源</span><span class="sxs-lookup"><span data-stu-id="cc20f-138">Content sources</span></span>|<span data-ttu-id="cc20f-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc20f-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="cc20f-140">参与策略</span><span class="sxs-lookup"><span data-stu-id="cc20f-140">Contributing policies</span></span>|
|<span data-ttu-id="cc20f-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="cc20f-141">currentValue</span></span>|<span data-ttu-id="cc20f-142">String</span><span class="sxs-lookup"><span data-stu-id="cc20f-142">String</span></span>|<span data-ttu-id="cc20f-143">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="cc20f-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc20f-144">关系</span><span class="sxs-lookup"><span data-stu-id="cc20f-144">Relationships</span></span>
<span data-ttu-id="cc20f-145">无</span><span class="sxs-lookup"><span data-stu-id="cc20f-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc20f-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc20f-146">JSON Representation</span></span>
<span data-ttu-id="cc20f-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc20f-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
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



