---
title: macOSFirewallApplication 资源类型
description: 代表 macOS 防火墙应用程序列表中的应用程序
ms.openlocfilehash: 6e016f2191fd9b366bbdf5dbaef5562284a6b5ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043158"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="350fa-103">macOSFirewallApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="350fa-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="350fa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="350fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="350fa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="350fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="350fa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="350fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="350fa-107">代表 macOS 防火墙应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="350fa-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="350fa-108">属性</span><span class="sxs-lookup"><span data-stu-id="350fa-108">Properties</span></span>
|<span data-ttu-id="350fa-109">属性</span><span class="sxs-lookup"><span data-stu-id="350fa-109">Property</span></span>|<span data-ttu-id="350fa-110">类型</span><span class="sxs-lookup"><span data-stu-id="350fa-110">Type</span></span>|<span data-ttu-id="350fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="350fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="350fa-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="350fa-112">bundleId</span></span>|<span data-ttu-id="350fa-113">String</span><span class="sxs-lookup"><span data-stu-id="350fa-113">String</span></span>|<span data-ttu-id="350fa-114">应用程序的 BundleId。</span><span class="sxs-lookup"><span data-stu-id="350fa-114">BundleId of the application.</span></span>|
|<span data-ttu-id="350fa-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="350fa-115">allowsIncomingConnections</span></span>|<span data-ttu-id="350fa-116">布尔</span><span class="sxs-lookup"><span data-stu-id="350fa-116">Boolean</span></span>|<span data-ttu-id="350fa-117">是否允许传入连接。</span><span class="sxs-lookup"><span data-stu-id="350fa-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="350fa-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="350fa-118">Relationships</span></span>
<span data-ttu-id="350fa-119">无</span><span class="sxs-lookup"><span data-stu-id="350fa-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="350fa-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="350fa-120">JSON Representation</span></span>
<span data-ttu-id="350fa-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="350fa-121">Here is a JSON representation of the resource.</span></span>
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





