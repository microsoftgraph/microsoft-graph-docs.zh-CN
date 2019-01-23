---
title: macOSFirewallApplication 资源类型
description: 代表 macOS 防火墙应用程序列表中的应用程序
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe3bbd83c3101420ec011fda85304fabce06daf0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404209"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="7a386-103">macOSFirewallApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a386-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="7a386-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7a386-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a386-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7a386-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a386-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a386-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a386-107">代表 macOS 防火墙应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="7a386-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="7a386-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a386-108">Properties</span></span>
|<span data-ttu-id="7a386-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a386-109">Property</span></span>|<span data-ttu-id="7a386-110">类型</span><span class="sxs-lookup"><span data-stu-id="7a386-110">Type</span></span>|<span data-ttu-id="7a386-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a386-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a386-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="7a386-112">bundleId</span></span>|<span data-ttu-id="7a386-113">String</span><span class="sxs-lookup"><span data-stu-id="7a386-113">String</span></span>|<span data-ttu-id="7a386-114">应用程序的 BundleId。</span><span class="sxs-lookup"><span data-stu-id="7a386-114">BundleId of the application.</span></span>|
|<span data-ttu-id="7a386-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="7a386-115">allowsIncomingConnections</span></span>|<span data-ttu-id="7a386-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a386-116">Boolean</span></span>|<span data-ttu-id="7a386-117">是否允许传入连接。</span><span class="sxs-lookup"><span data-stu-id="7a386-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a386-118">关系</span><span class="sxs-lookup"><span data-stu-id="7a386-118">Relationships</span></span>
<span data-ttu-id="7a386-119">无</span><span class="sxs-lookup"><span data-stu-id="7a386-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a386-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a386-120">JSON Representation</span></span>
<span data-ttu-id="7a386-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a386-121">Here is a JSON representation of the resource.</span></span>
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




