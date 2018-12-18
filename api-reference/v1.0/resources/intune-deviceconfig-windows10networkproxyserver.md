---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: tfitzmac
ms.openlocfilehash: c2eaeaa4d89f981e5fa992e7a79a7863f0848a9f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344035"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="0f009-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f009-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="0f009-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0f009-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f009-105">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="0f009-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="0f009-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f009-106">Properties</span></span>
|<span data-ttu-id="0f009-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f009-107">Property</span></span>|<span data-ttu-id="0f009-108">类型</span><span class="sxs-lookup"><span data-stu-id="0f009-108">Type</span></span>|<span data-ttu-id="0f009-109">说明</span><span class="sxs-lookup"><span data-stu-id="0f009-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f009-110">address</span><span class="sxs-lookup"><span data-stu-id="0f009-110">address</span></span>|<span data-ttu-id="0f009-111">String</span><span class="sxs-lookup"><span data-stu-id="0f009-111">String</span></span>|<span data-ttu-id="0f009-112">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="0f009-112">Address to the proxy server.</span></span> <span data-ttu-id="0f009-113">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="0f009-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="0f009-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="0f009-114">exceptions</span></span>|<span data-ttu-id="0f009-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f009-115">String collection</span></span>|<span data-ttu-id="0f009-116">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="0f009-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="0f009-117">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="0f009-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="0f009-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="0f009-118">useForLocalAddresses</span></span>|<span data-ttu-id="0f009-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f009-119">Boolean</span></span>|<span data-ttu-id="0f009-120">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="0f009-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f009-121">关系</span><span class="sxs-lookup"><span data-stu-id="0f009-121">Relationships</span></span>
<span data-ttu-id="0f009-122">无</span><span class="sxs-lookup"><span data-stu-id="0f009-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f009-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f009-123">JSON Representation</span></span>
<span data-ttu-id="0f009-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f009-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



