---
title: macOSFirewallApplication 资源类型
description: 表示 macOS 防火墙应用程序列表中的应用程序
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eb1f77bdadf62ddf6ac5362653ddb7d535f8c85
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946182"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="5ad71-103">macOSFirewallApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ad71-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="5ad71-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ad71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ad71-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ad71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ad71-106">表示 macOS 防火墙应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="5ad71-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="5ad71-107">属性</span><span class="sxs-lookup"><span data-stu-id="5ad71-107">Properties</span></span>
|<span data-ttu-id="5ad71-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ad71-108">Property</span></span>|<span data-ttu-id="5ad71-109">类型</span><span class="sxs-lookup"><span data-stu-id="5ad71-109">Type</span></span>|<span data-ttu-id="5ad71-110">说明</span><span class="sxs-lookup"><span data-stu-id="5ad71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ad71-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="5ad71-111">bundleId</span></span>|<span data-ttu-id="5ad71-112">String</span><span class="sxs-lookup"><span data-stu-id="5ad71-112">String</span></span>|<span data-ttu-id="5ad71-113">应用程序的 BundleId。</span><span class="sxs-lookup"><span data-stu-id="5ad71-113">BundleId of the application.</span></span>|
|<span data-ttu-id="5ad71-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="5ad71-114">allowsIncomingConnections</span></span>|<span data-ttu-id="5ad71-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ad71-115">Boolean</span></span>|<span data-ttu-id="5ad71-116">是否允许传入连接。</span><span class="sxs-lookup"><span data-stu-id="5ad71-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ad71-117">关系</span><span class="sxs-lookup"><span data-stu-id="5ad71-117">Relationships</span></span>
<span data-ttu-id="5ad71-118">无</span><span class="sxs-lookup"><span data-stu-id="5ad71-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ad71-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ad71-119">JSON Representation</span></span>
<span data-ttu-id="5ad71-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ad71-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```




