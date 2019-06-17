---
title: deviceManagementTroubleshootingErrorResource 资源类型
description: 表示指向疑难解答信息的链接的对象, 则该链接可能指向 Azure 门户或 Microsoft doc。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6aa8493638a4cdcc486cce0a0036328a2ff359e1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988186"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="2c87b-103">deviceManagementTroubleshootingErrorResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c87b-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="2c87b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c87b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c87b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c87b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c87b-106">表示指向疑难解答信息的链接的对象, 则该链接可能指向 Azure 门户或 Microsoft doc。</span><span class="sxs-lookup"><span data-stu-id="2c87b-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="2c87b-107">属性</span><span class="sxs-lookup"><span data-stu-id="2c87b-107">Properties</span></span>
|<span data-ttu-id="2c87b-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c87b-108">Property</span></span>|<span data-ttu-id="2c87b-109">类型</span><span class="sxs-lookup"><span data-stu-id="2c87b-109">Type</span></span>|<span data-ttu-id="2c87b-110">说明</span><span class="sxs-lookup"><span data-stu-id="2c87b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c87b-111">text</span><span class="sxs-lookup"><span data-stu-id="2c87b-111">text</span></span>|<span data-ttu-id="2c87b-112">String</span><span class="sxs-lookup"><span data-stu-id="2c87b-112">String</span></span>|<span data-ttu-id="2c87b-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2c87b-113">Not yet documented</span></span>|
|<span data-ttu-id="2c87b-114">link</span><span class="sxs-lookup"><span data-stu-id="2c87b-114">link</span></span>|<span data-ttu-id="2c87b-115">String</span><span class="sxs-lookup"><span data-stu-id="2c87b-115">String</span></span>|<span data-ttu-id="2c87b-116">指向 web 资源的链接。</span><span class="sxs-lookup"><span data-stu-id="2c87b-116">The link to the web resource.</span></span> <span data-ttu-id="2c87b-117">可以包含以下任何格式化程序: {{UPN}}、{{DeviceGUID}}、{{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="2c87b-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c87b-118">关系</span><span class="sxs-lookup"><span data-stu-id="2c87b-118">Relationships</span></span>
<span data-ttu-id="2c87b-119">无</span><span class="sxs-lookup"><span data-stu-id="2c87b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c87b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c87b-120">JSON Representation</span></span>
<span data-ttu-id="2c87b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c87b-121">Here is a JSON representation of the resource.</span></span>
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





