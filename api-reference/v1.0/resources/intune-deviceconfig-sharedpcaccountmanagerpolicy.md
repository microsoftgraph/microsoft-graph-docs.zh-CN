---
title: sharedPCAccountManagerPolicy 资源类型
description: 共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f23590e168090a48cb054fa5952faec893761d30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027816"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="d8924-104">sharedPCAccountManagerPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8924-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="d8924-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8924-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8924-106">共享电脑帐户管理器策略</span><span class="sxs-lookup"><span data-stu-id="d8924-106">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="d8924-107">仅在启用了帐户管理器时适用。</span><span class="sxs-lookup"><span data-stu-id="d8924-107">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="d8924-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8924-108">Properties</span></span>
|<span data-ttu-id="d8924-109">属性</span><span class="sxs-lookup"><span data-stu-id="d8924-109">Property</span></span>|<span data-ttu-id="d8924-110">类型</span><span class="sxs-lookup"><span data-stu-id="d8924-110">Type</span></span>|<span data-ttu-id="d8924-111">说明</span><span class="sxs-lookup"><span data-stu-id="d8924-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8924-112">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="d8924-112">accountDeletionPolicy</span></span>|[<span data-ttu-id="d8924-113">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="d8924-113">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="d8924-114">配置何时删除帐户。</span><span class="sxs-lookup"><span data-stu-id="d8924-114">Configures when accounts are deleted.</span></span> <span data-ttu-id="d8924-115">可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。</span><span class="sxs-lookup"><span data-stu-id="d8924-115">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="d8924-116">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="d8924-116">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="d8924-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d8924-117">Int32</span></span>|<span data-ttu-id="d8924-118">设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="d8924-118">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="d8924-119">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="d8924-119">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="d8924-120">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="d8924-120">Valid values 0 to 100</span></span>|
|<span data-ttu-id="d8924-121">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="d8924-121">inactiveThresholdDays</span></span>|<span data-ttu-id="d8924-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d8924-122">Int32</span></span>|<span data-ttu-id="d8924-123">指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。</span><span class="sxs-lookup"><span data-stu-id="d8924-123">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="d8924-124">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="d8924-124">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="d8924-125">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="d8924-125">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="d8924-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d8924-126">Int32</span></span>|<span data-ttu-id="d8924-127">设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="d8924-127">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="d8924-128">将首先删除处于非活动状态时间最长的帐户。</span><span class="sxs-lookup"><span data-stu-id="d8924-128">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="d8924-129">仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="d8924-129">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="d8924-130">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="d8924-130">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8924-131">关系</span><span class="sxs-lookup"><span data-stu-id="d8924-131">Relationships</span></span>
<span data-ttu-id="d8924-132">无</span><span class="sxs-lookup"><span data-stu-id="d8924-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8924-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8924-133">JSON Representation</span></span>
<span data-ttu-id="d8924-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8924-134">Here is a JSON representation of the resource.</span></span>
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



