---
title: vpnRoute 资源类型
description: VPN 路由定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43924b76a76060ac6576657d172757a503204a82
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927588"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="dc263-103">vpnRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc263-103">vpnRoute resource type</span></span>

> <span data-ttu-id="dc263-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dc263-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc263-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dc263-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc263-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dc263-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc263-107">VPN 路由定义。</span><span class="sxs-lookup"><span data-stu-id="dc263-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="dc263-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc263-108">Properties</span></span>
|<span data-ttu-id="dc263-109">属性</span><span class="sxs-lookup"><span data-stu-id="dc263-109">Property</span></span>|<span data-ttu-id="dc263-110">类型</span><span class="sxs-lookup"><span data-stu-id="dc263-110">Type</span></span>|<span data-ttu-id="dc263-111">Description</span><span class="sxs-lookup"><span data-stu-id="dc263-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc263-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="dc263-112">destinationPrefix</span></span>|<span data-ttu-id="dc263-113">字符串</span><span class="sxs-lookup"><span data-stu-id="dc263-113">String</span></span>|<span data-ttu-id="dc263-114">目标前缀 （IPv4/v6 地址）。</span><span class="sxs-lookup"><span data-stu-id="dc263-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="dc263-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="dc263-115">prefixSize</span></span>|<span data-ttu-id="dc263-116">Int32</span><span class="sxs-lookup"><span data-stu-id="dc263-116">Int32</span></span>|<span data-ttu-id="dc263-117">前缀大小。</span><span class="sxs-lookup"><span data-stu-id="dc263-117">Prefix size.</span></span> <span data-ttu-id="dc263-118">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="dc263-118">(1-32).</span></span> <span data-ttu-id="dc263-119">有效的值 1 到 32</span><span class="sxs-lookup"><span data-stu-id="dc263-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc263-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="dc263-120">Relationships</span></span>
<span data-ttu-id="dc263-121">无</span><span class="sxs-lookup"><span data-stu-id="dc263-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc263-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc263-122">JSON Representation</span></span>
<span data-ttu-id="dc263-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc263-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```





