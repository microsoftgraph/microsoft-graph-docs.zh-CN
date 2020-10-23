---
title: sharedAppleDeviceUser 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3946247ba9424fb1c961a11753376b7bcfb78c4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724450"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="13562-103">sharedAppleDeviceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="13562-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="13562-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13562-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13562-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13562-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13562-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13562-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13562-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13562-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="13562-108">属性</span><span class="sxs-lookup"><span data-stu-id="13562-108">Properties</span></span>
|<span data-ttu-id="13562-109">属性</span><span class="sxs-lookup"><span data-stu-id="13562-109">Property</span></span>|<span data-ttu-id="13562-110">类型</span><span class="sxs-lookup"><span data-stu-id="13562-110">Type</span></span>|<span data-ttu-id="13562-111">说明</span><span class="sxs-lookup"><span data-stu-id="13562-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13562-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13562-112">userPrincipalName</span></span>|<span data-ttu-id="13562-113">String</span><span class="sxs-lookup"><span data-stu-id="13562-113">String</span></span>|<span data-ttu-id="13562-114">用户名</span><span class="sxs-lookup"><span data-stu-id="13562-114">User name</span></span>|
|<span data-ttu-id="13562-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="13562-115">dataToSync</span></span>|<span data-ttu-id="13562-116">布尔</span><span class="sxs-lookup"><span data-stu-id="13562-116">Boolean</span></span>|<span data-ttu-id="13562-117">要同步的数据</span><span class="sxs-lookup"><span data-stu-id="13562-117">Data to sync</span></span>|
|<span data-ttu-id="13562-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="13562-118">dataQuota</span></span>|<span data-ttu-id="13562-119">Int64</span><span class="sxs-lookup"><span data-stu-id="13562-119">Int64</span></span>|<span data-ttu-id="13562-120">数据配额</span><span class="sxs-lookup"><span data-stu-id="13562-120">Data quota</span></span>|
|<span data-ttu-id="13562-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="13562-121">dataUsed</span></span>|<span data-ttu-id="13562-122">Int64</span><span class="sxs-lookup"><span data-stu-id="13562-122">Int64</span></span>|<span data-ttu-id="13562-123">数据配额</span><span class="sxs-lookup"><span data-stu-id="13562-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="13562-124">关系</span><span class="sxs-lookup"><span data-stu-id="13562-124">Relationships</span></span>
<span data-ttu-id="13562-125">无</span><span class="sxs-lookup"><span data-stu-id="13562-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13562-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13562-126">JSON Representation</span></span>
<span data-ttu-id="13562-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13562-127">Here is a JSON representation of the resource.</span></span>
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





