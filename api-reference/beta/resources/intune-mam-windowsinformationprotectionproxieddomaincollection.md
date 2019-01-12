---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a2f4b1e29afd113c2e06b611fabd525f9f5a6ba1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916899"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="ed64e-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed64e-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="ed64e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ed64e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed64e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ed64e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed64e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ed64e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed64e-107">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="ed64e-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="ed64e-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed64e-108">Properties</span></span>
|<span data-ttu-id="ed64e-109">属性</span><span class="sxs-lookup"><span data-stu-id="ed64e-109">Property</span></span>|<span data-ttu-id="ed64e-110">类型</span><span class="sxs-lookup"><span data-stu-id="ed64e-110">Type</span></span>|<span data-ttu-id="ed64e-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed64e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed64e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ed64e-112">displayName</span></span>|<span data-ttu-id="ed64e-113">String</span><span class="sxs-lookup"><span data-stu-id="ed64e-113">String</span></span>|<span data-ttu-id="ed64e-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="ed64e-114">Display name</span></span>|
|<span data-ttu-id="ed64e-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="ed64e-115">proxiedDomains</span></span>|<span data-ttu-id="ed64e-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed64e-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="ed64e-117">代理域集合</span><span class="sxs-lookup"><span data-stu-id="ed64e-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed64e-118">关系</span><span class="sxs-lookup"><span data-stu-id="ed64e-118">Relationships</span></span>
<span data-ttu-id="ed64e-119">无</span><span class="sxs-lookup"><span data-stu-id="ed64e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed64e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed64e-120">JSON Representation</span></span>
<span data-ttu-id="ed64e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed64e-121">Here is a JSON representation of the resource.</span></span>
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





