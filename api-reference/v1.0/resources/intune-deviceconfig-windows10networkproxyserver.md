---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c409c5d9db30d01acbd080d4bc38f96b22d3534a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451567"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="c9d22-103">windows10NetworkProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9d22-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="c9d22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9d22-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9d22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9d22-106">网络代理服务器策略。</span><span class="sxs-lookup"><span data-stu-id="c9d22-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="c9d22-107">属性</span><span class="sxs-lookup"><span data-stu-id="c9d22-107">Properties</span></span>
|<span data-ttu-id="c9d22-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9d22-108">Property</span></span>|<span data-ttu-id="c9d22-109">类型</span><span class="sxs-lookup"><span data-stu-id="c9d22-109">Type</span></span>|<span data-ttu-id="c9d22-110">说明</span><span class="sxs-lookup"><span data-stu-id="c9d22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9d22-111">address</span><span class="sxs-lookup"><span data-stu-id="c9d22-111">address</span></span>|<span data-ttu-id="c9d22-112">String</span><span class="sxs-lookup"><span data-stu-id="c9d22-112">String</span></span>|<span data-ttu-id="c9d22-113">代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="c9d22-113">Address to the proxy server.</span></span> <span data-ttu-id="c9d22-114">在 "\>\[服务器：\<端口" \<格式中指定地址\>\]</span><span class="sxs-lookup"><span data-stu-id="c9d22-114">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="c9d22-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="c9d22-115">exceptions</span></span>|<span data-ttu-id="c9d22-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="c9d22-116">String collection</span></span>|<span data-ttu-id="c9d22-117">不应使用代理服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="c9d22-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="c9d22-118">系统无法将代理服务器用于以本节点中指定的内容开头的地址。</span><span class="sxs-lookup"><span data-stu-id="c9d22-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="c9d22-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="c9d22-119">useForLocalAddresses</span></span>|<span data-ttu-id="c9d22-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d22-120">Boolean</span></span>|<span data-ttu-id="c9d22-121">指定是否应将代理服务器用于本地 (Intranet) 地址。</span><span class="sxs-lookup"><span data-stu-id="c9d22-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9d22-122">关系</span><span class="sxs-lookup"><span data-stu-id="c9d22-122">Relationships</span></span>
<span data-ttu-id="c9d22-123">无</span><span class="sxs-lookup"><span data-stu-id="c9d22-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9d22-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9d22-124">JSON Representation</span></span>
<span data-ttu-id="c9d22-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9d22-125">Here is a JSON representation of the resource.</span></span>
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







