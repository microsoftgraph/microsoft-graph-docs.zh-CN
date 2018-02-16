# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="7e762-101">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e762-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="7e762-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7e762-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e762-103">充当所有设备应用管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="7e762-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="7e762-104">方法</span><span class="sxs-lookup"><span data-stu-id="7e762-104">Methods</span></span>
|<span data-ttu-id="7e762-105">方法</span><span class="sxs-lookup"><span data-stu-id="7e762-105">Method</span></span>|<span data-ttu-id="7e762-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e762-106">Return Type</span></span>|<span data-ttu-id="7e762-107">说明</span><span class="sxs-lookup"><span data-stu-id="7e762-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e762-108">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7e762-108">Get deviceAppManagement</span></span>](../api/intune_onboarding_deviceappmanagement_get.md)|[<span data-ttu-id="7e762-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7e762-109">deviceAppManagement</span></span>](../resources/intune_onboarding_deviceappmanagement.md)|<span data-ttu-id="7e762-110">读取 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e762-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="7e762-111">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7e762-111">Update deviceAppManagement</span></span>](../api/intune_onboarding_deviceappmanagement_update.md)|[<span data-ttu-id="7e762-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7e762-112">deviceAppManagement</span></span>](../resources/intune_onboarding_deviceappmanagement.md)|<span data-ttu-id="7e762-113">更新 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e762-113">Update the properties of a [calendar](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="7e762-114">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="7e762-114">syncMicrosoftStoreForBusinessApps action</span></span>](../api/intune_onboarding_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md)|<span data-ttu-id="7e762-115">无</span><span class="sxs-lookup"><span data-stu-id="7e762-115">None</span></span>|<span data-ttu-id="7e762-116">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="7e762-116">Syncs Intune account with Microsoft Store For Business</span></span>|

## <a name="properties"></a><span data-ttu-id="7e762-117">属性</span><span class="sxs-lookup"><span data-stu-id="7e762-117">Properties</span></span>
|<span data-ttu-id="7e762-118">属性</span><span class="sxs-lookup"><span data-stu-id="7e762-118">Property</span></span>|<span data-ttu-id="7e762-119">类型</span><span class="sxs-lookup"><span data-stu-id="7e762-119">Type</span></span>|<span data-ttu-id="7e762-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e762-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e762-121">id</span><span class="sxs-lookup"><span data-stu-id="7e762-121">id</span></span>|<span data-ttu-id="7e762-122">String</span><span class="sxs-lookup"><span data-stu-id="7e762-122">String</span></span>|<span data-ttu-id="7e762-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7e762-123">Not yet documented</span></span>|
|<span data-ttu-id="7e762-124">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7e762-124">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="7e762-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e762-125">DateTimeOffset</span></span>|<span data-ttu-id="7e762-126">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="7e762-126">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="7e762-127">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="7e762-127">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="7e762-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e762-128">Boolean</span></span>|<span data-ttu-id="7e762-129">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="7e762-129">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="7e762-130">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="7e762-130">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="7e762-131">String</span><span class="sxs-lookup"><span data-stu-id="7e762-131">String</span></span>|<span data-ttu-id="7e762-132">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="7e762-132">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="7e762-133">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="7e762-133">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="7e762-134">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="7e762-134">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="7e762-135">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="7e762-135">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="7e762-136">例如，“en-US”为英国（美国）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="7e762-136">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="7e762-137">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="7e762-137">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="7e762-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e762-138">DateTimeOffset</span></span>|<span data-ttu-id="7e762-139">从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。</span><span class="sxs-lookup"><span data-stu-id="7e762-139">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e762-140">关系</span><span class="sxs-lookup"><span data-stu-id="7e762-140">Relationships</span></span>
<span data-ttu-id="7e762-141">无</span><span class="sxs-lookup"><span data-stu-id="7e762-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e762-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e762-142">JSON Representation</span></span>
<span data-ttu-id="7e762-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e762-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



