---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
ms.openlocfilehash: dc924d75bc2cf1310cb715033281f59b70abb32a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320291"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="eaf2c-103">proxiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="eaf2c-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="eaf2c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eaf2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaf2c-105">代理域</span><span class="sxs-lookup"><span data-stu-id="eaf2c-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="eaf2c-106">属性</span><span class="sxs-lookup"><span data-stu-id="eaf2c-106">Properties</span></span>
|<span data-ttu-id="eaf2c-107">属性</span><span class="sxs-lookup"><span data-stu-id="eaf2c-107">Property</span></span>|<span data-ttu-id="eaf2c-108">类型</span><span class="sxs-lookup"><span data-stu-id="eaf2c-108">Type</span></span>|<span data-ttu-id="eaf2c-109">说明</span><span class="sxs-lookup"><span data-stu-id="eaf2c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf2c-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="eaf2c-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="eaf2c-111">String</span><span class="sxs-lookup"><span data-stu-id="eaf2c-111">String</span></span>|<span data-ttu-id="eaf2c-112">IP 地址或 FQDN</span><span class="sxs-lookup"><span data-stu-id="eaf2c-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="eaf2c-113">代理</span><span class="sxs-lookup"><span data-stu-id="eaf2c-113">proxy</span></span>|<span data-ttu-id="eaf2c-114">String</span><span class="sxs-lookup"><span data-stu-id="eaf2c-114">String</span></span>|<span data-ttu-id="eaf2c-115">代理 IP</span><span class="sxs-lookup"><span data-stu-id="eaf2c-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaf2c-116">关系</span><span class="sxs-lookup"><span data-stu-id="eaf2c-116">Relationships</span></span>
<span data-ttu-id="eaf2c-117">无</span><span class="sxs-lookup"><span data-stu-id="eaf2c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eaf2c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eaf2c-118">JSON Representation</span></span>
<span data-ttu-id="eaf2c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaf2c-119">Here is a JSON representation of the resource.</span></span>
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



