---
title: deviceManagementTroubleshootingErrorResource 资源类型
description: 表示指向疑难解答信息的链接的对象，则该链接可能指向 Azure 门户或 Microsoft doc。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18537e1fa81fd082cc7fd78d2675540535195a32
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075782"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="c4074-103">deviceManagementTroubleshootingErrorResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4074-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

<span data-ttu-id="c4074-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4074-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4074-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4074-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4074-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4074-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4074-107">表示指向疑难解答信息的链接的对象，则该链接可能指向 Azure 门户或 Microsoft doc。</span><span class="sxs-lookup"><span data-stu-id="c4074-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="c4074-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4074-108">Properties</span></span>
|<span data-ttu-id="c4074-109">属性</span><span class="sxs-lookup"><span data-stu-id="c4074-109">Property</span></span>|<span data-ttu-id="c4074-110">类型</span><span class="sxs-lookup"><span data-stu-id="c4074-110">Type</span></span>|<span data-ttu-id="c4074-111">说明</span><span class="sxs-lookup"><span data-stu-id="c4074-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4074-112">text</span><span class="sxs-lookup"><span data-stu-id="c4074-112">text</span></span>|<span data-ttu-id="c4074-113">String</span><span class="sxs-lookup"><span data-stu-id="c4074-113">String</span></span>|<span data-ttu-id="c4074-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4074-114">Not yet documented</span></span>|
|<span data-ttu-id="c4074-115">link</span><span class="sxs-lookup"><span data-stu-id="c4074-115">link</span></span>|<span data-ttu-id="c4074-116">String</span><span class="sxs-lookup"><span data-stu-id="c4074-116">String</span></span>|<span data-ttu-id="c4074-117">指向 web 资源的链接。</span><span class="sxs-lookup"><span data-stu-id="c4074-117">The link to the web resource.</span></span> <span data-ttu-id="c4074-118">可以包含以下任何格式化程序： {{UPN}}、{{DeviceGUID}}、{{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="c4074-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4074-119">关系</span><span class="sxs-lookup"><span data-stu-id="c4074-119">Relationships</span></span>
<span data-ttu-id="c4074-120">无</span><span class="sxs-lookup"><span data-stu-id="c4074-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4074-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4074-121">JSON Representation</span></span>
<span data-ttu-id="c4074-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4074-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```






