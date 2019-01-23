---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a4b6a94f317c5d75b440aeef7fe387496be32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421674"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="fb3ca-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb3ca-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="fb3ca-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fb3ca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb3ca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb3ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb3ca-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb3ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb3ca-107">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="fb3ca-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="fb3ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb3ca-108">Properties</span></span>
|<span data-ttu-id="fb3ca-109">属性</span><span class="sxs-lookup"><span data-stu-id="fb3ca-109">Property</span></span>|<span data-ttu-id="fb3ca-110">类型</span><span class="sxs-lookup"><span data-stu-id="fb3ca-110">Type</span></span>|<span data-ttu-id="fb3ca-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb3ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb3ca-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fb3ca-112">displayName</span></span>|<span data-ttu-id="fb3ca-113">String</span><span class="sxs-lookup"><span data-stu-id="fb3ca-113">String</span></span>|<span data-ttu-id="fb3ca-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="fb3ca-114">Display name</span></span>|
|<span data-ttu-id="fb3ca-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="fb3ca-115">proxiedDomains</span></span>|<span data-ttu-id="fb3ca-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fb3ca-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="fb3ca-117">代理域集合</span><span class="sxs-lookup"><span data-stu-id="fb3ca-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb3ca-118">关系</span><span class="sxs-lookup"><span data-stu-id="fb3ca-118">Relationships</span></span>
<span data-ttu-id="fb3ca-119">无</span><span class="sxs-lookup"><span data-stu-id="fb3ca-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb3ca-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb3ca-120">JSON Representation</span></span>
<span data-ttu-id="fb3ca-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb3ca-121">Here is a JSON representation of the resource.</span></span>
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




