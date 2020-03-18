---
title: androidDeviceOwnerGlobalProxyAutoConfig 资源类型
description: Android 设备所有者全局代理自动配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c3acf7ef749a95cd17009284d587e4dd41ef4ec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797012"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="ec60d-103">androidDeviceOwnerGlobalProxyAutoConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec60d-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

> <span data-ttu-id="ec60d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec60d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec60d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec60d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec60d-106">Android 设备所有者全局代理自动配置。</span><span class="sxs-lookup"><span data-stu-id="ec60d-106">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="ec60d-107">继承自[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="ec60d-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec60d-108">属性</span><span class="sxs-lookup"><span data-stu-id="ec60d-108">Properties</span></span>
|<span data-ttu-id="ec60d-109">属性</span><span class="sxs-lookup"><span data-stu-id="ec60d-109">Property</span></span>|<span data-ttu-id="ec60d-110">类型</span><span class="sxs-lookup"><span data-stu-id="ec60d-110">Type</span></span>|<span data-ttu-id="ec60d-111">说明</span><span class="sxs-lookup"><span data-stu-id="ec60d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec60d-112">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="ec60d-112">proxyAutoConfigURL</span></span>|<span data-ttu-id="ec60d-113">String</span><span class="sxs-lookup"><span data-stu-id="ec60d-113">String</span></span>|<span data-ttu-id="ec60d-114">代理自动配置 URL</span><span class="sxs-lookup"><span data-stu-id="ec60d-114">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec60d-115">关系</span><span class="sxs-lookup"><span data-stu-id="ec60d-115">Relationships</span></span>
<span data-ttu-id="ec60d-116">无</span><span class="sxs-lookup"><span data-stu-id="ec60d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec60d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec60d-117">JSON Representation</span></span>
<span data-ttu-id="ec60d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec60d-118">Here is a JSON representation of the resource.</span></span>
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



