---
title: sharedPCAccountManagerPolicy 资源类型
description: 共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ae3ab06e52d3a6e9757841999907afadd02e137
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787535"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="fd1a5-104">sharedPCAccountManagerPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd1a5-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="fd1a5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd1a5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd1a5-107">共享电脑帐户管理器策略</span><span class="sxs-lookup"><span data-stu-id="fd1a5-107">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="fd1a5-108">仅在启用了帐户管理器时适用。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-108">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="fd1a5-109">属性</span><span class="sxs-lookup"><span data-stu-id="fd1a5-109">Properties</span></span>
|<span data-ttu-id="fd1a5-110">属性</span><span class="sxs-lookup"><span data-stu-id="fd1a5-110">Property</span></span>|<span data-ttu-id="fd1a5-111">类型</span><span class="sxs-lookup"><span data-stu-id="fd1a5-111">Type</span></span>|<span data-ttu-id="fd1a5-112">说明</span><span class="sxs-lookup"><span data-stu-id="fd1a5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd1a5-113">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd1a5-113">accountDeletionPolicy</span></span>|[<span data-ttu-id="fd1a5-114">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="fd1a5-114">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="fd1a5-115">配置何时删除帐户。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-115">Configures when accounts are deleted.</span></span> <span data-ttu-id="fd1a5-116">可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-116">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="fd1a5-117">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="fd1a5-117">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="fd1a5-118">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1a5-118">Int32</span></span>|<span data-ttu-id="fd1a5-119">设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-119">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="fd1a5-120">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-120">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="fd1a5-121">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="fd1a5-121">Valid values 0 to 100</span></span>|
|<span data-ttu-id="fd1a5-122">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="fd1a5-122">inactiveThresholdDays</span></span>|<span data-ttu-id="fd1a5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1a5-123">Int32</span></span>|<span data-ttu-id="fd1a5-124">指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-124">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="fd1a5-125">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-125">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="fd1a5-126">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="fd1a5-126">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="fd1a5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1a5-127">Int32</span></span>|<span data-ttu-id="fd1a5-128">设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-128">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="fd1a5-129">将首先删除处于非活动状态时间最长的帐户。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-129">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="fd1a5-130">仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-130">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="fd1a5-131">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="fd1a5-131">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd1a5-132">关系</span><span class="sxs-lookup"><span data-stu-id="fd1a5-132">Relationships</span></span>
<span data-ttu-id="fd1a5-133">无</span><span class="sxs-lookup"><span data-stu-id="fd1a5-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd1a5-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd1a5-134">JSON Representation</span></span>
<span data-ttu-id="fd1a5-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd1a5-135">Here is a JSON representation of the resource.</span></span>
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



