---
title: macOSAssociatedDomainsItem 资源类型
description: 应用程序标识符到关联域的映射。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b14cc5fe7c13bbcdde94733c41caf2b68c0451e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268935"
---
# <a name="macosassociateddomainsitem-resource-type"></a><span data-ttu-id="328e0-103">macOSAssociatedDomainsItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="328e0-103">macOSAssociatedDomainsItem resource type</span></span>

<span data-ttu-id="328e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="328e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="328e0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="328e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="328e0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="328e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="328e0-107">应用程序标识符到关联域的映射。</span><span class="sxs-lookup"><span data-stu-id="328e0-107">A mapping of application identifiers to associated domains.</span></span>

## <a name="properties"></a><span data-ttu-id="328e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="328e0-108">Properties</span></span>
|<span data-ttu-id="328e0-109">属性</span><span class="sxs-lookup"><span data-stu-id="328e0-109">Property</span></span>|<span data-ttu-id="328e0-110">类型</span><span class="sxs-lookup"><span data-stu-id="328e0-110">Type</span></span>|<span data-ttu-id="328e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="328e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="328e0-112">applicationIdentifier</span><span class="sxs-lookup"><span data-stu-id="328e0-112">applicationIdentifier</span></span>|<span data-ttu-id="328e0-113">字符串</span><span class="sxs-lookup"><span data-stu-id="328e0-113">String</span></span>|<span data-ttu-id="328e0-114">要与域关联的应用程序的应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="328e0-114">The application identifier of the app to associate domains with.</span></span>|
|<span data-ttu-id="328e0-115">域</span><span class="sxs-lookup"><span data-stu-id="328e0-115">domains</span></span>|<span data-ttu-id="328e0-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="328e0-116">String collection</span></span>|<span data-ttu-id="328e0-117">要关联的域的列表。</span><span class="sxs-lookup"><span data-stu-id="328e0-117">The list of domains to associate.</span></span>|
|<span data-ttu-id="328e0-118">directDownloadsEnabled</span><span class="sxs-lookup"><span data-stu-id="328e0-118">directDownloadsEnabled</span></span>|<span data-ttu-id="328e0-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="328e0-119">Boolean</span></span>|<span data-ttu-id="328e0-120">确定是应直接下载数据还是通过 CDN 下载数据。</span><span class="sxs-lookup"><span data-stu-id="328e0-120">Determines whether data should be downloaded directly or via a CDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="328e0-121">关系</span><span class="sxs-lookup"><span data-stu-id="328e0-121">Relationships</span></span>
<span data-ttu-id="328e0-122">无</span><span class="sxs-lookup"><span data-stu-id="328e0-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="328e0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="328e0-123">JSON Representation</span></span>
<span data-ttu-id="328e0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="328e0-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsItem",
  "applicationIdentifier": "String",
  "domains": [
    "String"
  ],
  "directDownloadsEnabled": true
}
```




