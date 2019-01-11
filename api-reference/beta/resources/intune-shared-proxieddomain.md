---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b25d40058f4f79add5875698777e23f658992e05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846772"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="f47e4-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="f47e4-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="f47e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f47e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f47e4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f47e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f47e4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f47e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f47e4-107">代理域</span><span class="sxs-lookup"><span data-stu-id="f47e4-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="f47e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f47e4-108">Properties</span></span>
|<span data-ttu-id="f47e4-109">属性</span><span class="sxs-lookup"><span data-stu-id="f47e4-109">Property</span></span>|<span data-ttu-id="f47e4-110">类型</span><span class="sxs-lookup"><span data-stu-id="f47e4-110">Type</span></span>|<span data-ttu-id="f47e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="f47e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f47e4-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="f47e4-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="f47e4-113">String</span><span class="sxs-lookup"><span data-stu-id="f47e4-113">String</span></span>|<span data-ttu-id="f47e4-114">IP 地址或完全限定的域名 (FQDN)。</span><span class="sxs-lookup"><span data-stu-id="f47e4-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="f47e4-115">代理</span><span class="sxs-lookup"><span data-stu-id="f47e4-115">proxy</span></span>|<span data-ttu-id="f47e4-116">String</span><span class="sxs-lookup"><span data-stu-id="f47e4-116">String</span></span>|<span data-ttu-id="f47e4-117">代理服务器 IP 地址或 FQDN。</span><span class="sxs-lookup"><span data-stu-id="f47e4-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f47e4-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="f47e4-118">Relationships</span></span>
<span data-ttu-id="f47e4-119">无</span><span class="sxs-lookup"><span data-stu-id="f47e4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f47e4-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f47e4-120">JSON Representation</span></span>
<span data-ttu-id="f47e4-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f47e4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



