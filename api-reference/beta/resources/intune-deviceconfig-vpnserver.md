---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: tfitzmac
ms.openlocfilehash: a8f0e6bd38f243d0066da231ef07d1723961987b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328775"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="e3554-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3554-103">vpnServer resource type</span></span>

> <span data-ttu-id="e3554-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e3554-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3554-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e3554-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3554-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e3554-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3554-107">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="e3554-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="e3554-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3554-108">Properties</span></span>
|<span data-ttu-id="e3554-109">属性</span><span class="sxs-lookup"><span data-stu-id="e3554-109">Property</span></span>|<span data-ttu-id="e3554-110">类型</span><span class="sxs-lookup"><span data-stu-id="e3554-110">Type</span></span>|<span data-ttu-id="e3554-111">说明</span><span class="sxs-lookup"><span data-stu-id="e3554-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3554-112">说明</span><span class="sxs-lookup"><span data-stu-id="e3554-112">description</span></span>|<span data-ttu-id="e3554-113">String</span><span class="sxs-lookup"><span data-stu-id="e3554-113">String</span></span>|<span data-ttu-id="e3554-114">说明。</span><span class="sxs-lookup"><span data-stu-id="e3554-114">Description.</span></span>|
|<span data-ttu-id="e3554-115">address</span><span class="sxs-lookup"><span data-stu-id="e3554-115">address</span></span>|<span data-ttu-id="e3554-116">String</span><span class="sxs-lookup"><span data-stu-id="e3554-116">String</span></span>|<span data-ttu-id="e3554-117">地址 （IP 地址、 FQDN 或 URL）</span><span class="sxs-lookup"><span data-stu-id="e3554-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="e3554-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="e3554-118">isDefaultServer</span></span>|<span data-ttu-id="e3554-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3554-119">Boolean</span></span>|<span data-ttu-id="e3554-120">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="e3554-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3554-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="e3554-121">Relationships</span></span>
<span data-ttu-id="e3554-122">无</span><span class="sxs-lookup"><span data-stu-id="e3554-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e3554-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3554-123">JSON Representation</span></span>
<span data-ttu-id="e3554-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3554-124">Here is a JSON representation of the resource.</span></span>
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





