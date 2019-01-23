---
title: deviceManagementTroubleshootingErrorResource 资源类型
description: 到 Azure 门户或 Microsoft doc 可能对象代表链接到故障排除信息的链接。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429574"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="07854-103">deviceManagementTroubleshootingErrorResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="07854-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="07854-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="07854-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07854-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="07854-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07854-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07854-107">到 Azure 门户或 Microsoft doc 可能对象代表链接到故障排除信息的链接。</span><span class="sxs-lookup"><span data-stu-id="07854-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="07854-108">属性</span><span class="sxs-lookup"><span data-stu-id="07854-108">Properties</span></span>
|<span data-ttu-id="07854-109">属性</span><span class="sxs-lookup"><span data-stu-id="07854-109">Property</span></span>|<span data-ttu-id="07854-110">类型</span><span class="sxs-lookup"><span data-stu-id="07854-110">Type</span></span>|<span data-ttu-id="07854-111">说明</span><span class="sxs-lookup"><span data-stu-id="07854-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07854-112">text</span><span class="sxs-lookup"><span data-stu-id="07854-112">text</span></span>|<span data-ttu-id="07854-113">String</span><span class="sxs-lookup"><span data-stu-id="07854-113">String</span></span>|<span data-ttu-id="07854-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="07854-114">Not yet documented</span></span>|
|<span data-ttu-id="07854-115">link</span><span class="sxs-lookup"><span data-stu-id="07854-115">link</span></span>|<span data-ttu-id="07854-116">String</span><span class="sxs-lookup"><span data-stu-id="07854-116">String</span></span>|<span data-ttu-id="07854-117">指向 web 资源的链接。</span><span class="sxs-lookup"><span data-stu-id="07854-117">The link to the web resource.</span></span> <span data-ttu-id="07854-118">可以包含任何以下格式化程序: {{UPN}} {{DeviceGUID}} {{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="07854-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="07854-119">关系</span><span class="sxs-lookup"><span data-stu-id="07854-119">Relationships</span></span>
<span data-ttu-id="07854-120">无</span><span class="sxs-lookup"><span data-stu-id="07854-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07854-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07854-121">JSON Representation</span></span>
<span data-ttu-id="07854-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07854-122">Here is a JSON representation of the resource.</span></span>
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




