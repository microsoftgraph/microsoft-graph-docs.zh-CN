---
title: androidDeviceOwnerGlobalProxyAutoConfig 资源类型
description: Android 设备所有者全局代理自动配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e15b3009537bd55eb7d4af6d93bbea3b53f3325a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538649"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="3183b-103">androidDeviceOwnerGlobalProxyAutoConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="3183b-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

> <span data-ttu-id="3183b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3183b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3183b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3183b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3183b-106">Android 设备所有者全局代理自动配置。</span><span class="sxs-lookup"><span data-stu-id="3183b-106">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="3183b-107">继承自[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="3183b-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3183b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3183b-108">Properties</span></span>
|<span data-ttu-id="3183b-109">属性</span><span class="sxs-lookup"><span data-stu-id="3183b-109">Property</span></span>|<span data-ttu-id="3183b-110">类型</span><span class="sxs-lookup"><span data-stu-id="3183b-110">Type</span></span>|<span data-ttu-id="3183b-111">说明</span><span class="sxs-lookup"><span data-stu-id="3183b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3183b-112">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="3183b-112">proxyAutoConfigURL</span></span>|<span data-ttu-id="3183b-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3183b-113">String</span></span>|<span data-ttu-id="3183b-114">代理自动配置 URL</span><span class="sxs-lookup"><span data-stu-id="3183b-114">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="3183b-115">关系</span><span class="sxs-lookup"><span data-stu-id="3183b-115">Relationships</span></span>
<span data-ttu-id="3183b-116">无</span><span class="sxs-lookup"><span data-stu-id="3183b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3183b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3183b-117">JSON Representation</span></span>
<span data-ttu-id="3183b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3183b-118">Here is a JSON representation of the resource.</span></span>
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



