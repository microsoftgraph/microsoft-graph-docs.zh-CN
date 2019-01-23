---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 673cfe99e9cafe1b57fde5c70b7059286a6cc554
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418580"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="d4e57-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4e57-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="d4e57-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d4e57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4e57-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4e57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4e57-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4e57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e57-107">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="d4e57-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="d4e57-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4e57-108">Properties</span></span>
|<span data-ttu-id="d4e57-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4e57-109">Property</span></span>|<span data-ttu-id="d4e57-110">类型</span><span class="sxs-lookup"><span data-stu-id="d4e57-110">Type</span></span>|<span data-ttu-id="d4e57-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4e57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e57-112">address</span><span class="sxs-lookup"><span data-stu-id="d4e57-112">address</span></span>|<span data-ttu-id="d4e57-113">String</span><span class="sxs-lookup"><span data-stu-id="d4e57-113">String</span></span>|<span data-ttu-id="d4e57-114">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="d4e57-114">Address to the proxy server.</span></span> <span data-ttu-id="d4e57-115">按照以下格式指定地址：<server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="d4e57-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="d4e57-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="d4e57-116">exceptions</span></span>|<span data-ttu-id="d4e57-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="d4e57-117">String collection</span></span>|<span data-ttu-id="d4e57-118">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="d4e57-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="d4e57-119">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="d4e57-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="d4e57-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="d4e57-120">useForLocalAddresses</span></span>|<span data-ttu-id="d4e57-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e57-121">Boolean</span></span>|<span data-ttu-id="d4e57-122">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="d4e57-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4e57-123">关系</span><span class="sxs-lookup"><span data-stu-id="d4e57-123">Relationships</span></span>
<span data-ttu-id="d4e57-124">无</span><span class="sxs-lookup"><span data-stu-id="d4e57-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4e57-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4e57-125">JSON Representation</span></span>
<span data-ttu-id="d4e57-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4e57-126">Here is a JSON representation of the resource.</span></span>
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




