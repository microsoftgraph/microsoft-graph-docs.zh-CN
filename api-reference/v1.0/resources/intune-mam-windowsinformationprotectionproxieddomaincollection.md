---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: tfitzmac
ms.openlocfilehash: c95c54c5bbfcc1b5202a0c56a6e3932b35ffac88
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309469"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="12b55-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="12b55-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="12b55-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12b55-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12b55-105">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="12b55-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="12b55-106">属性</span><span class="sxs-lookup"><span data-stu-id="12b55-106">Properties</span></span>
|<span data-ttu-id="12b55-107">属性</span><span class="sxs-lookup"><span data-stu-id="12b55-107">Property</span></span>|<span data-ttu-id="12b55-108">类型</span><span class="sxs-lookup"><span data-stu-id="12b55-108">Type</span></span>|<span data-ttu-id="12b55-109">说明</span><span class="sxs-lookup"><span data-stu-id="12b55-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12b55-110">displayName</span><span class="sxs-lookup"><span data-stu-id="12b55-110">displayName</span></span>|<span data-ttu-id="12b55-111">String</span><span class="sxs-lookup"><span data-stu-id="12b55-111">String</span></span>|<span data-ttu-id="12b55-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="12b55-112">Display name</span></span>|
|<span data-ttu-id="12b55-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="12b55-113">proxiedDomains</span></span>|<span data-ttu-id="12b55-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12b55-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="12b55-115">代理域集合</span><span class="sxs-lookup"><span data-stu-id="12b55-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="12b55-116">关系</span><span class="sxs-lookup"><span data-stu-id="12b55-116">Relationships</span></span>
<span data-ttu-id="12b55-117">无</span><span class="sxs-lookup"><span data-stu-id="12b55-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12b55-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12b55-118">JSON Representation</span></span>
<span data-ttu-id="12b55-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12b55-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



