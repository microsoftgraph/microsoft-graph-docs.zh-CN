---
title: sharedAppleDeviceUser 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d6142b47205640e64b8e422b1727fdf60ac8a2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524912"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f6d79-103">sharedAppleDeviceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6d79-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="f6d79-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f6d79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6d79-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6d79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d79-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6d79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d79-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6d79-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f6d79-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6d79-108">Properties</span></span>
|<span data-ttu-id="f6d79-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6d79-109">Property</span></span>|<span data-ttu-id="f6d79-110">类型</span><span class="sxs-lookup"><span data-stu-id="f6d79-110">Type</span></span>|<span data-ttu-id="f6d79-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6d79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d79-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6d79-112">userPrincipalName</span></span>|<span data-ttu-id="f6d79-113">String</span><span class="sxs-lookup"><span data-stu-id="f6d79-113">String</span></span>|<span data-ttu-id="f6d79-114">用户名</span><span class="sxs-lookup"><span data-stu-id="f6d79-114">User name</span></span>|
|<span data-ttu-id="f6d79-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="f6d79-115">dataToSync</span></span>|<span data-ttu-id="f6d79-116">布尔</span><span class="sxs-lookup"><span data-stu-id="f6d79-116">Boolean</span></span>|<span data-ttu-id="f6d79-117">要同步的数据</span><span class="sxs-lookup"><span data-stu-id="f6d79-117">Data to sync</span></span>|
|<span data-ttu-id="f6d79-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="f6d79-118">dataQuota</span></span>|<span data-ttu-id="f6d79-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f6d79-119">Int64</span></span>|<span data-ttu-id="f6d79-120">数据配额</span><span class="sxs-lookup"><span data-stu-id="f6d79-120">Data quota</span></span>|
|<span data-ttu-id="f6d79-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="f6d79-121">dataUsed</span></span>|<span data-ttu-id="f6d79-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f6d79-122">Int64</span></span>|<span data-ttu-id="f6d79-123">数据配额</span><span class="sxs-lookup"><span data-stu-id="f6d79-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6d79-124">关系</span><span class="sxs-lookup"><span data-stu-id="f6d79-124">Relationships</span></span>
<span data-ttu-id="f6d79-125">无</span><span class="sxs-lookup"><span data-stu-id="f6d79-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6d79-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6d79-126">JSON Representation</span></span>
<span data-ttu-id="f6d79-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6d79-127">Here is a JSON representation of the resource.</span></span>
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



