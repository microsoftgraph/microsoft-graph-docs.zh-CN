---
title: sharedPCAccountManagerPolicy 资源类型
description: 共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 49026651cb2f6ff95cea24f5cd3a4b91686c4063
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460026"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="a9946-104">sharedPCAccountManagerPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9946-104">sharedPCAccountManagerPolicy resource type</span></span>

<span data-ttu-id="a9946-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9946-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9946-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9946-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9946-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9946-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9946-108">共享电脑帐户管理器策略</span><span class="sxs-lookup"><span data-stu-id="a9946-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="a9946-109">仅在启用了帐户管理器时适用。</span><span class="sxs-lookup"><span data-stu-id="a9946-109">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="a9946-110">属性</span><span class="sxs-lookup"><span data-stu-id="a9946-110">Properties</span></span>
|<span data-ttu-id="a9946-111">属性</span><span class="sxs-lookup"><span data-stu-id="a9946-111">Property</span></span>|<span data-ttu-id="a9946-112">类型</span><span class="sxs-lookup"><span data-stu-id="a9946-112">Type</span></span>|<span data-ttu-id="a9946-113">说明</span><span class="sxs-lookup"><span data-stu-id="a9946-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9946-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="a9946-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="a9946-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a9946-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="a9946-116">配置何时删除帐户。</span><span class="sxs-lookup"><span data-stu-id="a9946-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="a9946-117">可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。</span><span class="sxs-lookup"><span data-stu-id="a9946-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="a9946-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="a9946-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="a9946-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a9946-119">Int32</span></span>|<span data-ttu-id="a9946-120">设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="a9946-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="a9946-121">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="a9946-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="a9946-122">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="a9946-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a9946-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="a9946-123">inactiveThresholdDays</span></span>|<span data-ttu-id="a9946-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a9946-124">Int32</span></span>|<span data-ttu-id="a9946-125">指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。</span><span class="sxs-lookup"><span data-stu-id="a9946-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="a9946-126">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="a9946-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="a9946-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="a9946-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="a9946-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a9946-128">Int32</span></span>|<span data-ttu-id="a9946-129">设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="a9946-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="a9946-130">将首先删除处于非活动状态时间最长的帐户。</span><span class="sxs-lookup"><span data-stu-id="a9946-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="a9946-131">仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="a9946-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="a9946-132">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="a9946-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9946-133">关系</span><span class="sxs-lookup"><span data-stu-id="a9946-133">Relationships</span></span>
<span data-ttu-id="a9946-134">无</span><span class="sxs-lookup"><span data-stu-id="a9946-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9946-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9946-135">JSON Representation</span></span>
<span data-ttu-id="a9946-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9946-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```



