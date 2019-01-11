---
title: macOSFirewallApplication 资源类型
description: 代表 macOS 防火墙应用程序列表中的应用程序
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 536f2f596286f6b5457557f575ba018c65001bfe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835216"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="c54ca-103">macOSFirewallApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="c54ca-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="c54ca-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c54ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c54ca-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c54ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c54ca-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c54ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c54ca-107">代表 macOS 防火墙应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="c54ca-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="c54ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="c54ca-108">Properties</span></span>
|<span data-ttu-id="c54ca-109">属性</span><span class="sxs-lookup"><span data-stu-id="c54ca-109">Property</span></span>|<span data-ttu-id="c54ca-110">类型</span><span class="sxs-lookup"><span data-stu-id="c54ca-110">Type</span></span>|<span data-ttu-id="c54ca-111">说明</span><span class="sxs-lookup"><span data-stu-id="c54ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c54ca-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="c54ca-112">bundleId</span></span>|<span data-ttu-id="c54ca-113">String</span><span class="sxs-lookup"><span data-stu-id="c54ca-113">String</span></span>|<span data-ttu-id="c54ca-114">应用程序的 BundleId。</span><span class="sxs-lookup"><span data-stu-id="c54ca-114">BundleId of the application.</span></span>|
|<span data-ttu-id="c54ca-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="c54ca-115">allowsIncomingConnections</span></span>|<span data-ttu-id="c54ca-116">布尔</span><span class="sxs-lookup"><span data-stu-id="c54ca-116">Boolean</span></span>|<span data-ttu-id="c54ca-117">是否允许传入连接。</span><span class="sxs-lookup"><span data-stu-id="c54ca-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c54ca-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="c54ca-118">Relationships</span></span>
<span data-ttu-id="c54ca-119">无</span><span class="sxs-lookup"><span data-stu-id="c54ca-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c54ca-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c54ca-120">JSON Representation</span></span>
<span data-ttu-id="c54ca-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c54ca-121">Here is a JSON representation of the resource.</span></span>
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





