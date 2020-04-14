---
title: customSubjectAlternativeName 资源类型
description: 自定义主题备用名称定义
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b88b5c6a393d994de5d393984ee339969b25ba6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453462"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="10b07-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="10b07-103">customSubjectAlternativeName resource type</span></span>

<span data-ttu-id="10b07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10b07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10b07-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10b07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10b07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10b07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10b07-107">自定义主题备用名称定义</span><span class="sxs-lookup"><span data-stu-id="10b07-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="10b07-108">属性</span><span class="sxs-lookup"><span data-stu-id="10b07-108">Properties</span></span>
|<span data-ttu-id="10b07-109">属性</span><span class="sxs-lookup"><span data-stu-id="10b07-109">Property</span></span>|<span data-ttu-id="10b07-110">类型</span><span class="sxs-lookup"><span data-stu-id="10b07-110">Type</span></span>|<span data-ttu-id="10b07-111">说明</span><span class="sxs-lookup"><span data-stu-id="10b07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10b07-112">sanType</span><span class="sxs-lookup"><span data-stu-id="10b07-112">sanType</span></span>|[<span data-ttu-id="10b07-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="10b07-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="10b07-114">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="10b07-114">Custom SAN Type.</span></span> <span data-ttu-id="10b07-115">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="10b07-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="10b07-116">name</span><span class="sxs-lookup"><span data-stu-id="10b07-116">name</span></span>|<span data-ttu-id="10b07-117">String</span><span class="sxs-lookup"><span data-stu-id="10b07-117">String</span></span>|<span data-ttu-id="10b07-118">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="10b07-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="10b07-119">关系</span><span class="sxs-lookup"><span data-stu-id="10b07-119">Relationships</span></span>
<span data-ttu-id="10b07-120">无</span><span class="sxs-lookup"><span data-stu-id="10b07-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10b07-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10b07-121">JSON Representation</span></span>
<span data-ttu-id="10b07-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10b07-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```



