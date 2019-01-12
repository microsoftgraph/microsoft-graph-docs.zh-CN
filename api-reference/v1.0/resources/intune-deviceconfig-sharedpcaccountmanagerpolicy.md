---
title: sharedPCAccountManagerPolicy 资源类型
description: 共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b094f4761680da2fbead6f522a297f6d6450c197
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937661"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="5df45-104">sharedPCAccountManagerPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="5df45-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="5df45-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5df45-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5df45-106">共享电脑帐户管理器策略</span><span class="sxs-lookup"><span data-stu-id="5df45-106">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="5df45-107">仅在启用了帐户管理器时适用。</span><span class="sxs-lookup"><span data-stu-id="5df45-107">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="5df45-108">属性</span><span class="sxs-lookup"><span data-stu-id="5df45-108">Properties</span></span>
|<span data-ttu-id="5df45-109">属性</span><span class="sxs-lookup"><span data-stu-id="5df45-109">Property</span></span>|<span data-ttu-id="5df45-110">类型</span><span class="sxs-lookup"><span data-stu-id="5df45-110">Type</span></span>|<span data-ttu-id="5df45-111">说明</span><span class="sxs-lookup"><span data-stu-id="5df45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df45-112">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="5df45-112">accountDeletionPolicy</span></span>|[<span data-ttu-id="5df45-113">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="5df45-113">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="5df45-114">配置何时删除帐户。</span><span class="sxs-lookup"><span data-stu-id="5df45-114">Configures when accounts are deleted.</span></span> <span data-ttu-id="5df45-115">可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。</span><span class="sxs-lookup"><span data-stu-id="5df45-115">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="5df45-116">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="5df45-116">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="5df45-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5df45-117">Int32</span></span>|<span data-ttu-id="5df45-118">设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="5df45-118">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="5df45-119">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="5df45-119">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="5df45-120">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="5df45-120">Valid values 0 to 100</span></span>|
|<span data-ttu-id="5df45-121">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="5df45-121">inactiveThresholdDays</span></span>|<span data-ttu-id="5df45-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5df45-122">Int32</span></span>|<span data-ttu-id="5df45-123">指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。</span><span class="sxs-lookup"><span data-stu-id="5df45-123">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="5df45-124">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="5df45-124">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="5df45-125">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="5df45-125">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="5df45-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5df45-126">Int32</span></span>|<span data-ttu-id="5df45-127">设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="5df45-127">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="5df45-128">将首先删除处于非活动状态时间最长的帐户。</span><span class="sxs-lookup"><span data-stu-id="5df45-128">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="5df45-129">仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="5df45-129">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="5df45-130">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="5df45-130">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="5df45-131">关系</span><span class="sxs-lookup"><span data-stu-id="5df45-131">Relationships</span></span>
<span data-ttu-id="5df45-132">无</span><span class="sxs-lookup"><span data-stu-id="5df45-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5df45-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5df45-133">JSON Representation</span></span>
<span data-ttu-id="5df45-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5df45-134">Here is a JSON representation of the resource.</span></span>
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



