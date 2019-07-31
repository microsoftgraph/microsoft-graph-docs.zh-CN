---
title: deviceManagementTroubleshootingErrorResource 资源类型
description: 表示指向疑难解答信息的链接的对象, 则该链接可能指向 Azure 门户或 Microsoft doc。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6454bad98938bc73d4cde8d48229f6146d07c0bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010303"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="bbfd8-103">deviceManagementTroubleshootingErrorResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="bbfd8-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="bbfd8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bbfd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbfd8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bbfd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbfd8-106">表示指向疑难解答信息的链接的对象, 则该链接可能指向 Azure 门户或 Microsoft doc。</span><span class="sxs-lookup"><span data-stu-id="bbfd8-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="bbfd8-107">属性</span><span class="sxs-lookup"><span data-stu-id="bbfd8-107">Properties</span></span>
|<span data-ttu-id="bbfd8-108">属性</span><span class="sxs-lookup"><span data-stu-id="bbfd8-108">Property</span></span>|<span data-ttu-id="bbfd8-109">类型</span><span class="sxs-lookup"><span data-stu-id="bbfd8-109">Type</span></span>|<span data-ttu-id="bbfd8-110">说明</span><span class="sxs-lookup"><span data-stu-id="bbfd8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbfd8-111">text</span><span class="sxs-lookup"><span data-stu-id="bbfd8-111">text</span></span>|<span data-ttu-id="bbfd8-112">String</span><span class="sxs-lookup"><span data-stu-id="bbfd8-112">String</span></span>|<span data-ttu-id="bbfd8-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bbfd8-113">Not yet documented</span></span>|
|<span data-ttu-id="bbfd8-114">link</span><span class="sxs-lookup"><span data-stu-id="bbfd8-114">link</span></span>|<span data-ttu-id="bbfd8-115">String</span><span class="sxs-lookup"><span data-stu-id="bbfd8-115">String</span></span>|<span data-ttu-id="bbfd8-116">指向 web 资源的链接。</span><span class="sxs-lookup"><span data-stu-id="bbfd8-116">The link to the web resource.</span></span> <span data-ttu-id="bbfd8-117">可以包含以下任何格式化程序: {{UPN}}、{{DeviceGUID}}、{{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="bbfd8-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbfd8-118">关系</span><span class="sxs-lookup"><span data-stu-id="bbfd8-118">Relationships</span></span>
<span data-ttu-id="bbfd8-119">无</span><span class="sxs-lookup"><span data-stu-id="bbfd8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbfd8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bbfd8-120">JSON Representation</span></span>
<span data-ttu-id="bbfd8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbfd8-121">Here is a JSON representation of the resource.</span></span>
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





