---
title: vpnServer 资源类型
description: VPN 服务器定义。
ms.openlocfilehash: e89cc562c3fe0f6b353199ca7de639053177ab1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044932"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="c01e4-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="c01e4-103">vpnServer resource type</span></span>

> <span data-ttu-id="c01e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c01e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c01e4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c01e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c01e4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c01e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c01e4-107">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="c01e4-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="c01e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="c01e4-108">Properties</span></span>
|<span data-ttu-id="c01e4-109">属性</span><span class="sxs-lookup"><span data-stu-id="c01e4-109">Property</span></span>|<span data-ttu-id="c01e4-110">类型</span><span class="sxs-lookup"><span data-stu-id="c01e4-110">Type</span></span>|<span data-ttu-id="c01e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="c01e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c01e4-112">说明</span><span class="sxs-lookup"><span data-stu-id="c01e4-112">description</span></span>|<span data-ttu-id="c01e4-113">String</span><span class="sxs-lookup"><span data-stu-id="c01e4-113">String</span></span>|<span data-ttu-id="c01e4-114">说明。</span><span class="sxs-lookup"><span data-stu-id="c01e4-114">Description.</span></span>|
|<span data-ttu-id="c01e4-115">address</span><span class="sxs-lookup"><span data-stu-id="c01e4-115">address</span></span>|<span data-ttu-id="c01e4-116">String</span><span class="sxs-lookup"><span data-stu-id="c01e4-116">String</span></span>|<span data-ttu-id="c01e4-117">地址 （IP 地址、 FQDN 或 URL）</span><span class="sxs-lookup"><span data-stu-id="c01e4-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="c01e4-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="c01e4-118">isDefaultServer</span></span>|<span data-ttu-id="c01e4-119">布尔</span><span class="sxs-lookup"><span data-stu-id="c01e4-119">Boolean</span></span>|<span data-ttu-id="c01e4-120">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="c01e4-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c01e4-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="c01e4-121">Relationships</span></span>
<span data-ttu-id="c01e4-122">无</span><span class="sxs-lookup"><span data-stu-id="c01e4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c01e4-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c01e4-123">JSON Representation</span></span>
<span data-ttu-id="c01e4-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c01e4-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```





