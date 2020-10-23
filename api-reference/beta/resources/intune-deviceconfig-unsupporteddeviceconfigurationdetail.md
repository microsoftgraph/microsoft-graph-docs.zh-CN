---
title: unsupportedDeviceConfigurationDetail 资源类型
description: 有关实体不受支持的原因的说明。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f033e30400e3c198f325507030b2267425ce8f80
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703795"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="839d5-103">unsupportedDeviceConfigurationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="839d5-103">unsupportedDeviceConfigurationDetail resource type</span></span>

<span data-ttu-id="839d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="839d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="839d5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="839d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="839d5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="839d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="839d5-107">有关实体不受支持的原因的说明。</span><span class="sxs-lookup"><span data-stu-id="839d5-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="839d5-108">属性</span><span class="sxs-lookup"><span data-stu-id="839d5-108">Properties</span></span>
|<span data-ttu-id="839d5-109">属性</span><span class="sxs-lookup"><span data-stu-id="839d5-109">Property</span></span>|<span data-ttu-id="839d5-110">类型</span><span class="sxs-lookup"><span data-stu-id="839d5-110">Type</span></span>|<span data-ttu-id="839d5-111">描述</span><span class="sxs-lookup"><span data-stu-id="839d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="839d5-112">message</span><span class="sxs-lookup"><span data-stu-id="839d5-112">message</span></span>|<span data-ttu-id="839d5-113">String</span><span class="sxs-lookup"><span data-stu-id="839d5-113">String</span></span>|<span data-ttu-id="839d5-114">一条消息，说明实体不受支持的原因。</span><span class="sxs-lookup"><span data-stu-id="839d5-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="839d5-115">PropertyName</span><span class="sxs-lookup"><span data-stu-id="839d5-115">propertyName</span></span>|<span data-ttu-id="839d5-116">String</span><span class="sxs-lookup"><span data-stu-id="839d5-116">String</span></span>|<span data-ttu-id="839d5-117">如果邮件与原始实体中的特定属性相关，则为该属性的名称。</span><span class="sxs-lookup"><span data-stu-id="839d5-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="839d5-118">关系</span><span class="sxs-lookup"><span data-stu-id="839d5-118">Relationships</span></span>
<span data-ttu-id="839d5-119">无</span><span class="sxs-lookup"><span data-stu-id="839d5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="839d5-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="839d5-120">JSON Representation</span></span>
<span data-ttu-id="839d5-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="839d5-121">Here is a JSON representation of the resource.</span></span>
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





