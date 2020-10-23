---
title: androidDeviceOwnerGlobalProxyDirect 资源类型
description: Android 设备所有者全局代理 Direct。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fdf7d25bf21ceef36a9ce4f6ce5733238c63dc80
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708912"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="77e79-103">androidDeviceOwnerGlobalProxyDirect 资源类型</span><span class="sxs-lookup"><span data-stu-id="77e79-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

<span data-ttu-id="77e79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77e79-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77e79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77e79-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77e79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77e79-107">Android 设备所有者全局代理 Direct。</span><span class="sxs-lookup"><span data-stu-id="77e79-107">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="77e79-108">继承自 [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="77e79-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="77e79-109">属性</span><span class="sxs-lookup"><span data-stu-id="77e79-109">Properties</span></span>
|<span data-ttu-id="77e79-110">属性</span><span class="sxs-lookup"><span data-stu-id="77e79-110">Property</span></span>|<span data-ttu-id="77e79-111">类型</span><span class="sxs-lookup"><span data-stu-id="77e79-111">Type</span></span>|<span data-ttu-id="77e79-112">说明</span><span class="sxs-lookup"><span data-stu-id="77e79-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77e79-113">host</span><span class="sxs-lookup"><span data-stu-id="77e79-113">host</span></span>|<span data-ttu-id="77e79-114">String</span><span class="sxs-lookup"><span data-stu-id="77e79-114">String</span></span>|<span data-ttu-id="77e79-115">主机名</span><span class="sxs-lookup"><span data-stu-id="77e79-115">The host name</span></span>|
|<span data-ttu-id="77e79-116">端口</span><span class="sxs-lookup"><span data-stu-id="77e79-116">port</span></span>|<span data-ttu-id="77e79-117">Int32</span><span class="sxs-lookup"><span data-stu-id="77e79-117">Int32</span></span>|<span data-ttu-id="77e79-118">端口</span><span class="sxs-lookup"><span data-stu-id="77e79-118">The port</span></span>|
|<span data-ttu-id="77e79-119">excludedHosts</span><span class="sxs-lookup"><span data-stu-id="77e79-119">excludedHosts</span></span>|<span data-ttu-id="77e79-120">String collection</span><span class="sxs-lookup"><span data-stu-id="77e79-120">String collection</span></span>|<span data-ttu-id="77e79-121">已排除的主机</span><span class="sxs-lookup"><span data-stu-id="77e79-121">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="77e79-122">关系</span><span class="sxs-lookup"><span data-stu-id="77e79-122">Relationships</span></span>
<span data-ttu-id="77e79-123">无</span><span class="sxs-lookup"><span data-stu-id="77e79-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77e79-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77e79-124">JSON Representation</span></span>
<span data-ttu-id="77e79-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77e79-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyDirect"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyDirect",
  "host": "String",
  "port": 1024,
  "excludedHosts": [
    "String"
  ]
}
```





