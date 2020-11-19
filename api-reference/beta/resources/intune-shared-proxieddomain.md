---
title: proxiedDomain 资源类型
description: 代理域
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b31786ac628d1f1abab5309f1ae327909dac7076
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258876"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="6d851-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d851-103">proxiedDomain resource type</span></span>

<span data-ttu-id="6d851-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d851-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d851-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d851-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d851-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d851-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d851-107">代理域</span><span class="sxs-lookup"><span data-stu-id="6d851-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="6d851-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d851-108">Properties</span></span>
|<span data-ttu-id="6d851-109">属性</span><span class="sxs-lookup"><span data-stu-id="6d851-109">Property</span></span>|<span data-ttu-id="6d851-110">类型</span><span class="sxs-lookup"><span data-stu-id="6d851-110">Type</span></span>|<span data-ttu-id="6d851-111">描述</span><span class="sxs-lookup"><span data-stu-id="6d851-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d851-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="6d851-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="6d851-113">String</span><span class="sxs-lookup"><span data-stu-id="6d851-113">String</span></span>|<span data-ttu-id="6d851-114">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="6d851-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="6d851-115">代理</span><span class="sxs-lookup"><span data-stu-id="6d851-115">proxy</span></span>|<span data-ttu-id="6d851-116">String</span><span class="sxs-lookup"><span data-stu-id="6d851-116">String</span></span>|<span data-ttu-id="6d851-117">代理 IP 或 FQDN</span><span class="sxs-lookup"><span data-stu-id="6d851-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d851-118">关系</span><span class="sxs-lookup"><span data-stu-id="6d851-118">Relationships</span></span>
<span data-ttu-id="6d851-119">无</span><span class="sxs-lookup"><span data-stu-id="6d851-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d851-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d851-120">JSON Representation</span></span>
<span data-ttu-id="6d851-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d851-121">Here is a JSON representation of the resource.</span></span>
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




