---
title: sharedAppleDeviceUser 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff51ad89600919fb1ed2c3bb506a53178ccdc445
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941749"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="d84ab-103">sharedAppleDeviceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="d84ab-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="d84ab-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d84ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d84ab-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d84ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d84ab-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d84ab-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d84ab-107">属性</span><span class="sxs-lookup"><span data-stu-id="d84ab-107">Properties</span></span>
|<span data-ttu-id="d84ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="d84ab-108">Property</span></span>|<span data-ttu-id="d84ab-109">类型</span><span class="sxs-lookup"><span data-stu-id="d84ab-109">Type</span></span>|<span data-ttu-id="d84ab-110">说明</span><span class="sxs-lookup"><span data-stu-id="d84ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d84ab-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d84ab-111">userPrincipalName</span></span>|<span data-ttu-id="d84ab-112">String</span><span class="sxs-lookup"><span data-stu-id="d84ab-112">String</span></span>|<span data-ttu-id="d84ab-113">用户名</span><span class="sxs-lookup"><span data-stu-id="d84ab-113">User name</span></span>|
|<span data-ttu-id="d84ab-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="d84ab-114">dataToSync</span></span>|<span data-ttu-id="d84ab-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d84ab-115">Boolean</span></span>|<span data-ttu-id="d84ab-116">要同步的数据</span><span class="sxs-lookup"><span data-stu-id="d84ab-116">Data to sync</span></span>|
|<span data-ttu-id="d84ab-117">dataQuota</span><span class="sxs-lookup"><span data-stu-id="d84ab-117">dataQuota</span></span>|<span data-ttu-id="d84ab-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d84ab-118">Int64</span></span>|<span data-ttu-id="d84ab-119">数据配额</span><span class="sxs-lookup"><span data-stu-id="d84ab-119">Data quota</span></span>|
|<span data-ttu-id="d84ab-120">dataUsed</span><span class="sxs-lookup"><span data-stu-id="d84ab-120">dataUsed</span></span>|<span data-ttu-id="d84ab-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d84ab-121">Int64</span></span>|<span data-ttu-id="d84ab-122">数据配额</span><span class="sxs-lookup"><span data-stu-id="d84ab-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="d84ab-123">关系</span><span class="sxs-lookup"><span data-stu-id="d84ab-123">Relationships</span></span>
<span data-ttu-id="d84ab-124">无</span><span class="sxs-lookup"><span data-stu-id="d84ab-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d84ab-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d84ab-125">JSON Representation</span></span>
<span data-ttu-id="d84ab-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d84ab-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```




