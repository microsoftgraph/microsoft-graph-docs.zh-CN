---
title: customSubjectAlternativeName 资源类型
description: 自定义的 Subject Alternative Name 定义
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 069cc1f6d93c785e4fc774d7988e0fc80febbb12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954118"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="d779d-103">customSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="d779d-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="d779d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d779d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d779d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d779d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d779d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d779d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d779d-107">自定义的 Subject Alternative Name 定义</span><span class="sxs-lookup"><span data-stu-id="d779d-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="d779d-108">属性</span><span class="sxs-lookup"><span data-stu-id="d779d-108">Properties</span></span>
|<span data-ttu-id="d779d-109">属性</span><span class="sxs-lookup"><span data-stu-id="d779d-109">Property</span></span>|<span data-ttu-id="d779d-110">类型</span><span class="sxs-lookup"><span data-stu-id="d779d-110">Type</span></span>|<span data-ttu-id="d779d-111">Description</span><span class="sxs-lookup"><span data-stu-id="d779d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d779d-112">sanType</span><span class="sxs-lookup"><span data-stu-id="d779d-112">sanType</span></span>|[<span data-ttu-id="d779d-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d779d-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d779d-114">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="d779d-114">Custom SAN Type.</span></span> <span data-ttu-id="d779d-115">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="d779d-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d779d-116">name</span><span class="sxs-lookup"><span data-stu-id="d779d-116">name</span></span>|<span data-ttu-id="d779d-117">字符串</span><span class="sxs-lookup"><span data-stu-id="d779d-117">String</span></span>|<span data-ttu-id="d779d-118">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="d779d-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="d779d-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="d779d-119">Relationships</span></span>
<span data-ttu-id="d779d-120">无</span><span class="sxs-lookup"><span data-stu-id="d779d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d779d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d779d-121">JSON Representation</span></span>
<span data-ttu-id="d779d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d779d-122">Here is a JSON representation of the resource.</span></span>
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





