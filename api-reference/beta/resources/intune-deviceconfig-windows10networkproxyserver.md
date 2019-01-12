---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c193c5b5d1ba61626bb348f52caf39ded58a77c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951913"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="b02f7-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="b02f7-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="b02f7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b02f7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b02f7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b02f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b02f7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b02f7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b02f7-107">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="b02f7-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="b02f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="b02f7-108">Properties</span></span>
|<span data-ttu-id="b02f7-109">属性</span><span class="sxs-lookup"><span data-stu-id="b02f7-109">Property</span></span>|<span data-ttu-id="b02f7-110">类型</span><span class="sxs-lookup"><span data-stu-id="b02f7-110">Type</span></span>|<span data-ttu-id="b02f7-111">说明</span><span class="sxs-lookup"><span data-stu-id="b02f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b02f7-112">address</span><span class="sxs-lookup"><span data-stu-id="b02f7-112">address</span></span>|<span data-ttu-id="b02f7-113">String</span><span class="sxs-lookup"><span data-stu-id="b02f7-113">String</span></span>|<span data-ttu-id="b02f7-114">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="b02f7-114">Address to the proxy server.</span></span> <span data-ttu-id="b02f7-115">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="b02f7-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="b02f7-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="b02f7-116">exceptions</span></span>|<span data-ttu-id="b02f7-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="b02f7-117">String collection</span></span>|<span data-ttu-id="b02f7-118">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="b02f7-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="b02f7-119">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="b02f7-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="b02f7-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="b02f7-120">useForLocalAddresses</span></span>|<span data-ttu-id="b02f7-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="b02f7-121">Boolean</span></span>|<span data-ttu-id="b02f7-122">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="b02f7-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b02f7-123">关系</span><span class="sxs-lookup"><span data-stu-id="b02f7-123">Relationships</span></span>
<span data-ttu-id="b02f7-124">无</span><span class="sxs-lookup"><span data-stu-id="b02f7-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b02f7-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b02f7-125">JSON Representation</span></span>
<span data-ttu-id="b02f7-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b02f7-126">Here is a JSON representation of the resource.</span></span>
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





