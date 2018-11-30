---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
ms.openlocfilehash: 4e2e995c8d66249e5c742343f74e18e87337bfaa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046989"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="9ef03-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ef03-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="9ef03-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ef03-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ef03-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ef03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ef03-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ef03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ef03-107">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="9ef03-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="9ef03-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ef03-108">Properties</span></span>
|<span data-ttu-id="9ef03-109">属性</span><span class="sxs-lookup"><span data-stu-id="9ef03-109">Property</span></span>|<span data-ttu-id="9ef03-110">类型</span><span class="sxs-lookup"><span data-stu-id="9ef03-110">Type</span></span>|<span data-ttu-id="9ef03-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ef03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef03-112">address</span><span class="sxs-lookup"><span data-stu-id="9ef03-112">address</span></span>|<span data-ttu-id="9ef03-113">String</span><span class="sxs-lookup"><span data-stu-id="9ef03-113">String</span></span>|<span data-ttu-id="9ef03-114">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="9ef03-114">Address to the proxy server.</span></span> <span data-ttu-id="9ef03-115">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="9ef03-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="9ef03-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="9ef03-116">exceptions</span></span>|<span data-ttu-id="9ef03-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ef03-117">String collection</span></span>|<span data-ttu-id="9ef03-118">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="9ef03-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="9ef03-119">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="9ef03-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="9ef03-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="9ef03-120">useForLocalAddresses</span></span>|<span data-ttu-id="9ef03-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ef03-121">Boolean</span></span>|<span data-ttu-id="9ef03-122">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="9ef03-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef03-123">关系</span><span class="sxs-lookup"><span data-stu-id="9ef03-123">Relationships</span></span>
<span data-ttu-id="9ef03-124">无</span><span class="sxs-lookup"><span data-stu-id="9ef03-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ef03-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ef03-125">JSON Representation</span></span>
<span data-ttu-id="9ef03-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ef03-126">Here is a JSON representation of the resource.</span></span>
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





