---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b68f13ab80544d591b22fc77ab35110302dc48ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031008"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="5b2f8-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b2f8-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="5b2f8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b2f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b2f8-105">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="5b2f8-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="5b2f8-106">属性</span><span class="sxs-lookup"><span data-stu-id="5b2f8-106">Properties</span></span>
|<span data-ttu-id="5b2f8-107">属性</span><span class="sxs-lookup"><span data-stu-id="5b2f8-107">Property</span></span>|<span data-ttu-id="5b2f8-108">类型</span><span class="sxs-lookup"><span data-stu-id="5b2f8-108">Type</span></span>|<span data-ttu-id="5b2f8-109">说明</span><span class="sxs-lookup"><span data-stu-id="5b2f8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b2f8-110">address</span><span class="sxs-lookup"><span data-stu-id="5b2f8-110">address</span></span>|<span data-ttu-id="5b2f8-111">String</span><span class="sxs-lookup"><span data-stu-id="5b2f8-111">String</span></span>|<span data-ttu-id="5b2f8-112">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="5b2f8-112">Address to the proxy server.</span></span> <span data-ttu-id="5b2f8-113">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="5b2f8-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="5b2f8-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="5b2f8-114">exceptions</span></span>|<span data-ttu-id="5b2f8-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="5b2f8-115">String collection</span></span>|<span data-ttu-id="5b2f8-116">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="5b2f8-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="5b2f8-117">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="5b2f8-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="5b2f8-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="5b2f8-118">useForLocalAddresses</span></span>|<span data-ttu-id="5b2f8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b2f8-119">Boolean</span></span>|<span data-ttu-id="5b2f8-120">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="5b2f8-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b2f8-121">关系</span><span class="sxs-lookup"><span data-stu-id="5b2f8-121">Relationships</span></span>
<span data-ttu-id="5b2f8-122">无</span><span class="sxs-lookup"><span data-stu-id="5b2f8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b2f8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b2f8-123">JSON Representation</span></span>
<span data-ttu-id="5b2f8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b2f8-124">Here is a JSON representation of the resource.</span></span>
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



