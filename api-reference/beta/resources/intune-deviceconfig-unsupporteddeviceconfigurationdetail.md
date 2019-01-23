---
title: unsupportedDeviceConfigurationDetail 资源类型
description: 为什么说实体是不受支持的说明。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c03bdb20fc4c48fa7820e09b9212bf73250599aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400387"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="7155a-103">unsupportedDeviceConfigurationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="7155a-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="7155a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7155a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7155a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7155a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7155a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7155a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7155a-107">为什么说实体是不受支持的说明。</span><span class="sxs-lookup"><span data-stu-id="7155a-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="7155a-108">属性</span><span class="sxs-lookup"><span data-stu-id="7155a-108">Properties</span></span>
|<span data-ttu-id="7155a-109">属性</span><span class="sxs-lookup"><span data-stu-id="7155a-109">Property</span></span>|<span data-ttu-id="7155a-110">类型</span><span class="sxs-lookup"><span data-stu-id="7155a-110">Type</span></span>|<span data-ttu-id="7155a-111">说明</span><span class="sxs-lookup"><span data-stu-id="7155a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7155a-112">message</span><span class="sxs-lookup"><span data-stu-id="7155a-112">message</span></span>|<span data-ttu-id="7155a-113">String</span><span class="sxs-lookup"><span data-stu-id="7155a-113">String</span></span>|<span data-ttu-id="7155a-114">解释 entity 为什么不受支持的一条消息。</span><span class="sxs-lookup"><span data-stu-id="7155a-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="7155a-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="7155a-115">propertyName</span></span>|<span data-ttu-id="7155a-116">String</span><span class="sxs-lookup"><span data-stu-id="7155a-116">String</span></span>|<span data-ttu-id="7155a-117">如果邮件与原始实体，则该属性的名称中的特定属性。</span><span class="sxs-lookup"><span data-stu-id="7155a-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7155a-118">关系</span><span class="sxs-lookup"><span data-stu-id="7155a-118">Relationships</span></span>
<span data-ttu-id="7155a-119">无</span><span class="sxs-lookup"><span data-stu-id="7155a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7155a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7155a-120">JSON Representation</span></span>
<span data-ttu-id="7155a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7155a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```




