---
title: androidDeviceOwnerGlobalProxyAutoConfig 资源类型
description: Android 设备所有者全局代理自动配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 207cbafb423b322fd954d561a4204150cb078abf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486596"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="ebbf8-103">androidDeviceOwnerGlobalProxyAutoConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebbf8-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="ebbf8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ebbf8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebbf8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebbf8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebbf8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebbf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebbf8-107">Android 设备所有者全局代理自动配置。</span><span class="sxs-lookup"><span data-stu-id="ebbf8-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="ebbf8-108">继承自[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="ebbf8-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebbf8-109">属性</span><span class="sxs-lookup"><span data-stu-id="ebbf8-109">Properties</span></span>
|<span data-ttu-id="ebbf8-110">属性</span><span class="sxs-lookup"><span data-stu-id="ebbf8-110">Property</span></span>|<span data-ttu-id="ebbf8-111">类型</span><span class="sxs-lookup"><span data-stu-id="ebbf8-111">Type</span></span>|<span data-ttu-id="ebbf8-112">说明</span><span class="sxs-lookup"><span data-stu-id="ebbf8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbf8-113">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="ebbf8-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="ebbf8-114">String</span><span class="sxs-lookup"><span data-stu-id="ebbf8-114">String</span></span>|<span data-ttu-id="ebbf8-115">代理自动配置 URL</span><span class="sxs-lookup"><span data-stu-id="ebbf8-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebbf8-116">关系</span><span class="sxs-lookup"><span data-stu-id="ebbf8-116">Relationships</span></span>
<span data-ttu-id="ebbf8-117">无</span><span class="sxs-lookup"><span data-stu-id="ebbf8-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebbf8-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebbf8-118">JSON Representation</span></span>
<span data-ttu-id="ebbf8-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebbf8-119">Here is a JSON representation of the resource.</span></span>
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



