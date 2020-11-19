---
title: sharedAppleDeviceUser 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4cd33eccfbc1c3e396d65f63a6f435690186b53f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208791"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="e8b7d-103">sharedAppleDeviceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8b7d-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="e8b7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8b7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8b7d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8b7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8b7d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8b7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8b7d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8b7d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e8b7d-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8b7d-108">Properties</span></span>
|<span data-ttu-id="e8b7d-109">属性</span><span class="sxs-lookup"><span data-stu-id="e8b7d-109">Property</span></span>|<span data-ttu-id="e8b7d-110">类型</span><span class="sxs-lookup"><span data-stu-id="e8b7d-110">Type</span></span>|<span data-ttu-id="e8b7d-111">说明</span><span class="sxs-lookup"><span data-stu-id="e8b7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8b7d-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e8b7d-112">userPrincipalName</span></span>|<span data-ttu-id="e8b7d-113">String</span><span class="sxs-lookup"><span data-stu-id="e8b7d-113">String</span></span>|<span data-ttu-id="e8b7d-114">用户名</span><span class="sxs-lookup"><span data-stu-id="e8b7d-114">User name</span></span>|
|<span data-ttu-id="e8b7d-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="e8b7d-115">dataToSync</span></span>|<span data-ttu-id="e8b7d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8b7d-116">Boolean</span></span>|<span data-ttu-id="e8b7d-117">要同步的数据</span><span class="sxs-lookup"><span data-stu-id="e8b7d-117">Data to sync</span></span>|
|<span data-ttu-id="e8b7d-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="e8b7d-118">dataQuota</span></span>|<span data-ttu-id="e8b7d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e8b7d-119">Int64</span></span>|<span data-ttu-id="e8b7d-120">数据配额</span><span class="sxs-lookup"><span data-stu-id="e8b7d-120">Data quota</span></span>|
|<span data-ttu-id="e8b7d-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="e8b7d-121">dataUsed</span></span>|<span data-ttu-id="e8b7d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e8b7d-122">Int64</span></span>|<span data-ttu-id="e8b7d-123">数据配额</span><span class="sxs-lookup"><span data-stu-id="e8b7d-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8b7d-124">关系</span><span class="sxs-lookup"><span data-stu-id="e8b7d-124">Relationships</span></span>
<span data-ttu-id="e8b7d-125">无</span><span class="sxs-lookup"><span data-stu-id="e8b7d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8b7d-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8b7d-126">JSON Representation</span></span>
<span data-ttu-id="e8b7d-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8b7d-127">Here is a JSON representation of the resource.</span></span>
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




