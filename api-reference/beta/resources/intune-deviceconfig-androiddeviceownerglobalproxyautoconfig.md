---
title: androidDeviceOwnerGlobalProxyAutoConfig 资源类型
description: Android 设备所有者全局代理自动配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70b2fc59c2136364af0f2023b17c9f888fad8b6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303536"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="6d0b0-103">androidDeviceOwnerGlobalProxyAutoConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d0b0-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="6d0b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d0b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d0b0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d0b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d0b0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d0b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d0b0-107">Android 设备所有者全局代理自动配置。</span><span class="sxs-lookup"><span data-stu-id="6d0b0-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="6d0b0-108">继承自 [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="6d0b0-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6d0b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="6d0b0-109">Properties</span></span>
|<span data-ttu-id="6d0b0-110">属性</span><span class="sxs-lookup"><span data-stu-id="6d0b0-110">Property</span></span>|<span data-ttu-id="6d0b0-111">类型</span><span class="sxs-lookup"><span data-stu-id="6d0b0-111">Type</span></span>|<span data-ttu-id="6d0b0-112">Description</span><span class="sxs-lookup"><span data-stu-id="6d0b0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d0b0-113">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="6d0b0-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="6d0b0-114">字符串</span><span class="sxs-lookup"><span data-stu-id="6d0b0-114">String</span></span>|<span data-ttu-id="6d0b0-115">代理自动配置 URL</span><span class="sxs-lookup"><span data-stu-id="6d0b0-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d0b0-116">关系</span><span class="sxs-lookup"><span data-stu-id="6d0b0-116">Relationships</span></span>
<span data-ttu-id="6d0b0-117">无</span><span class="sxs-lookup"><span data-stu-id="6d0b0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d0b0-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d0b0-118">JSON Representation</span></span>
<span data-ttu-id="6d0b0-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d0b0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
  "proxyAutoConfigURL": "String"
}
```




