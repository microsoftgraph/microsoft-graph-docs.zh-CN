---
title: proxiedDomain 资源类型
description: 代理域
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6079a2503004a1606e9db0e4b20dce8725f37ab9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474101"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="2a6ca-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a6ca-103">proxiedDomain resource type</span></span>

<span data-ttu-id="2a6ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a6ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a6ca-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a6ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a6ca-106">代理域</span><span class="sxs-lookup"><span data-stu-id="2a6ca-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="2a6ca-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a6ca-107">Properties</span></span>
|<span data-ttu-id="2a6ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a6ca-108">Property</span></span>|<span data-ttu-id="2a6ca-109">类型</span><span class="sxs-lookup"><span data-stu-id="2a6ca-109">Type</span></span>|<span data-ttu-id="2a6ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a6ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a6ca-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="2a6ca-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="2a6ca-112">String</span><span class="sxs-lookup"><span data-stu-id="2a6ca-112">String</span></span>|<span data-ttu-id="2a6ca-113">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="2a6ca-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="2a6ca-114">代理</span><span class="sxs-lookup"><span data-stu-id="2a6ca-114">proxy</span></span>|<span data-ttu-id="2a6ca-115">String</span><span class="sxs-lookup"><span data-stu-id="2a6ca-115">String</span></span>|<span data-ttu-id="2a6ca-116">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="2a6ca-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a6ca-117">关系</span><span class="sxs-lookup"><span data-stu-id="2a6ca-117">Relationships</span></span>
<span data-ttu-id="2a6ca-118">无</span><span class="sxs-lookup"><span data-stu-id="2a6ca-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a6ca-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a6ca-119">JSON Representation</span></span>
<span data-ttu-id="2a6ca-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a6ca-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```







