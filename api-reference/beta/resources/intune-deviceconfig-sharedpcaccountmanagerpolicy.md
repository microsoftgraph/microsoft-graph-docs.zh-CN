---
title: sharedPCAccountManagerPolicy 资源类型
description: 共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b8824f3f9b18722f69db4f3d0d116b2f46dfd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914883"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="2d771-104">sharedPCAccountManagerPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d771-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="2d771-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2d771-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d771-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2d771-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d771-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2d771-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d771-108">共享电脑帐户管理器策略</span><span class="sxs-lookup"><span data-stu-id="2d771-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="2d771-109">仅在启用了帐户管理器时适用。</span><span class="sxs-lookup"><span data-stu-id="2d771-109">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="2d771-110">属性</span><span class="sxs-lookup"><span data-stu-id="2d771-110">Properties</span></span>
|<span data-ttu-id="2d771-111">属性</span><span class="sxs-lookup"><span data-stu-id="2d771-111">Property</span></span>|<span data-ttu-id="2d771-112">类型</span><span class="sxs-lookup"><span data-stu-id="2d771-112">Type</span></span>|<span data-ttu-id="2d771-113">说明</span><span class="sxs-lookup"><span data-stu-id="2d771-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d771-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="2d771-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="2d771-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2d771-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="2d771-116">配置何时删除帐户。</span><span class="sxs-lookup"><span data-stu-id="2d771-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="2d771-117">可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。</span><span class="sxs-lookup"><span data-stu-id="2d771-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="2d771-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="2d771-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="2d771-119">Int32</span><span class="sxs-lookup"><span data-stu-id="2d771-119">Int32</span></span>|<span data-ttu-id="2d771-120">设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="2d771-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="2d771-121">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="2d771-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="2d771-122">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="2d771-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="2d771-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="2d771-123">inactiveThresholdDays</span></span>|<span data-ttu-id="2d771-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2d771-124">Int32</span></span>|<span data-ttu-id="2d771-125">指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。</span><span class="sxs-lookup"><span data-stu-id="2d771-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="2d771-126">仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="2d771-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="2d771-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="2d771-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="2d771-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2d771-128">Int32</span></span>|<span data-ttu-id="2d771-129">设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。</span><span class="sxs-lookup"><span data-stu-id="2d771-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="2d771-130">将首先删除处于非活动状态时间最长的帐户。</span><span class="sxs-lookup"><span data-stu-id="2d771-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="2d771-131">仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。</span><span class="sxs-lookup"><span data-stu-id="2d771-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="2d771-132">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="2d771-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d771-133">关系</span><span class="sxs-lookup"><span data-stu-id="2d771-133">Relationships</span></span>
<span data-ttu-id="2d771-134">无</span><span class="sxs-lookup"><span data-stu-id="2d771-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d771-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d771-135">JSON Representation</span></span>
<span data-ttu-id="2d771-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d771-136">Here is a JSON representation of the resource.</span></span>
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





