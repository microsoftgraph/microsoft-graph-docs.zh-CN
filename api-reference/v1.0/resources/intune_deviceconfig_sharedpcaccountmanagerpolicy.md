# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="2d367-101">sharedPCAccountManagerPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d367-101">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="2d367-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2d367-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d367-103">共享电脑帐户管理器策略</span><span class="sxs-lookup"><span data-stu-id="2d367-103">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="2d367-104">仅在启用了帐户管理器时适用。</span><span class="sxs-lookup"><span data-stu-id="2d367-104">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="2d367-105">属性</span><span class="sxs-lookup"><span data-stu-id="2d367-105">Properties</span></span>
|<span data-ttu-id="2d367-106">属性</span><span class="sxs-lookup"><span data-stu-id="2d367-106">Property</span></span>|<span data-ttu-id="2d367-107">类型</span><span class="sxs-lookup"><span data-stu-id="2d367-107">Type</span></span>|<span data-ttu-id="2d367-108">说明</span><span class="sxs-lookup"><span data-stu-id="2d367-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d367-109">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="2d367-109">accountDeletionPolicy</span></span>|[<span data-ttu-id="2d367-110">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2d367-110">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune_deviceconfig_sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="2d367-111">配置何时删除帐户。</span><span class="sxs-lookup"><span data-stu-id="2d367-111">Configures when accounts are deleted.</span></span> <span data-ttu-id="2d367-112">可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。</span><span class="sxs-lookup"><span data-stu-id="2d367-112">The possible values are `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="2d367-113">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="2d367-113">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="2d367-114">Int32</span><span class="sxs-lookup"><span data-stu-id="2d367-114">Int32</span></span>|<span data-ttu-id="2d367-115">设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="2d367-115">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="2d367-116">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="2d367-116">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="2d367-117">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="2d367-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="2d367-118">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="2d367-118">inactiveThresholdDays</span></span>|<span data-ttu-id="2d367-119">Int32</span><span class="sxs-lookup"><span data-stu-id="2d367-119">Int32</span></span>|<span data-ttu-id="2d367-120">指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。</span><span class="sxs-lookup"><span data-stu-id="2d367-120">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="2d367-121">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="2d367-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="2d367-122">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="2d367-122">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="2d367-123">Int32</span><span class="sxs-lookup"><span data-stu-id="2d367-123">Int32</span></span>|<span data-ttu-id="2d367-124">设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="2d367-124">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="2d367-125">将首先删除处于非活动状态时间最长的帐户。</span><span class="sxs-lookup"><span data-stu-id="2d367-125">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="2d367-126">仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="2d367-126">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="2d367-127">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="2d367-127">Valid values 0 to 100</span></span>|


## <a name="relationships"></a><span data-ttu-id="2d367-128">关系</span><span class="sxs-lookup"><span data-stu-id="2d367-128">Relationships</span></span>
<span data-ttu-id="2d367-129">无</span><span class="sxs-lookup"><span data-stu-id="2d367-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d367-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d367-130">JSON Representation</span></span>
<span data-ttu-id="2d367-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d367-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```



