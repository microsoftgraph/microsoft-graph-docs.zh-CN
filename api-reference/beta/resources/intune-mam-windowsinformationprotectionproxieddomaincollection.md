---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
ms.openlocfilehash: 07539361d99211f2a787fe538745debf09fa4cf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047431"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="1f974-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f974-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="1f974-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1f974-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f974-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1f974-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f974-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f974-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f974-107">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="1f974-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="1f974-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f974-108">Properties</span></span>
|<span data-ttu-id="1f974-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f974-109">Property</span></span>|<span data-ttu-id="1f974-110">类型</span><span class="sxs-lookup"><span data-stu-id="1f974-110">Type</span></span>|<span data-ttu-id="1f974-111">说明</span><span class="sxs-lookup"><span data-stu-id="1f974-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f974-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1f974-112">displayName</span></span>|<span data-ttu-id="1f974-113">String</span><span class="sxs-lookup"><span data-stu-id="1f974-113">String</span></span>|<span data-ttu-id="1f974-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="1f974-114">Display name</span></span>|
|<span data-ttu-id="1f974-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="1f974-115">proxiedDomains</span></span>|<span data-ttu-id="1f974-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1f974-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="1f974-117">代理域集合</span><span class="sxs-lookup"><span data-stu-id="1f974-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f974-118">关系</span><span class="sxs-lookup"><span data-stu-id="1f974-118">Relationships</span></span>
<span data-ttu-id="1f974-119">无</span><span class="sxs-lookup"><span data-stu-id="1f974-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f974-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f974-120">JSON Representation</span></span>
<span data-ttu-id="1f974-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f974-121">Here is a JSON representation of the resource.</span></span>
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





