---
title: customSubjectAlternativeName 资源类型
description: 自定义的 Subject Alternative Name 定义
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3f081b37b79be45d6705d24be58ea7295b58b68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415668"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="cfd6b-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfd6b-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="cfd6b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cfd6b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cfd6b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cfd6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfd6b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cfd6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfd6b-107">自定义的 Subject Alternative Name 定义</span><span class="sxs-lookup"><span data-stu-id="cfd6b-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="cfd6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cfd6b-108">Properties</span></span>
|<span data-ttu-id="cfd6b-109">属性</span><span class="sxs-lookup"><span data-stu-id="cfd6b-109">Property</span></span>|<span data-ttu-id="cfd6b-110">类型</span><span class="sxs-lookup"><span data-stu-id="cfd6b-110">Type</span></span>|<span data-ttu-id="cfd6b-111">说明</span><span class="sxs-lookup"><span data-stu-id="cfd6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfd6b-112">sanType</span><span class="sxs-lookup"><span data-stu-id="cfd6b-112">sanType</span></span>|[<span data-ttu-id="cfd6b-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cfd6b-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="cfd6b-114">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="cfd6b-114">Custom SAN Type.</span></span> <span data-ttu-id="cfd6b-115">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="cfd6b-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="cfd6b-116">name</span><span class="sxs-lookup"><span data-stu-id="cfd6b-116">name</span></span>|<span data-ttu-id="cfd6b-117">String</span><span class="sxs-lookup"><span data-stu-id="cfd6b-117">String</span></span>|<span data-ttu-id="cfd6b-118">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="cfd6b-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfd6b-119">关系</span><span class="sxs-lookup"><span data-stu-id="cfd6b-119">Relationships</span></span>
<span data-ttu-id="cfd6b-120">无</span><span class="sxs-lookup"><span data-stu-id="cfd6b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfd6b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfd6b-121">JSON Representation</span></span>
<span data-ttu-id="cfd6b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfd6b-122">Here is a JSON representation of the resource.</span></span>
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




