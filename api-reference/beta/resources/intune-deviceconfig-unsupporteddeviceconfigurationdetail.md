---
title: unsupportedDeviceConfigurationDetail 资源类型
description: 有关实体不受支持的原因的说明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce838f73c4ad02ecb29d540a9f0d4af065796993
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978967"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="2eee3-103">unsupportedDeviceConfigurationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="2eee3-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="2eee3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2eee3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eee3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2eee3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eee3-106">有关实体不受支持的原因的说明。</span><span class="sxs-lookup"><span data-stu-id="2eee3-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="2eee3-107">属性</span><span class="sxs-lookup"><span data-stu-id="2eee3-107">Properties</span></span>
|<span data-ttu-id="2eee3-108">属性</span><span class="sxs-lookup"><span data-stu-id="2eee3-108">Property</span></span>|<span data-ttu-id="2eee3-109">类型</span><span class="sxs-lookup"><span data-stu-id="2eee3-109">Type</span></span>|<span data-ttu-id="2eee3-110">描述</span><span class="sxs-lookup"><span data-stu-id="2eee3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eee3-111">message</span><span class="sxs-lookup"><span data-stu-id="2eee3-111">message</span></span>|<span data-ttu-id="2eee3-112">String</span><span class="sxs-lookup"><span data-stu-id="2eee3-112">String</span></span>|<span data-ttu-id="2eee3-113">一条消息, 说明实体不受支持的原因。</span><span class="sxs-lookup"><span data-stu-id="2eee3-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="2eee3-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="2eee3-114">propertyName</span></span>|<span data-ttu-id="2eee3-115">String</span><span class="sxs-lookup"><span data-stu-id="2eee3-115">String</span></span>|<span data-ttu-id="2eee3-116">如果邮件与原始实体中的特定属性相关, 则为该属性的名称。</span><span class="sxs-lookup"><span data-stu-id="2eee3-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2eee3-117">关系</span><span class="sxs-lookup"><span data-stu-id="2eee3-117">Relationships</span></span>
<span data-ttu-id="2eee3-118">无</span><span class="sxs-lookup"><span data-stu-id="2eee3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2eee3-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2eee3-119">JSON Representation</span></span>
<span data-ttu-id="2eee3-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2eee3-120">Here is a JSON representation of the resource.</span></span>
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





