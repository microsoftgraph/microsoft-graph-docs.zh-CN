---
title: windows10XCustomSubjectAlternativeName 资源类型
description: " (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 725d2cc13db1cb28b9286479f201b9bb38f6eefa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301503"
---
# <a name="windows10xcustomsubjectalternativename-resource-type"></a><span data-ttu-id="78dba-103">windows10XCustomSubjectAlternativeName 资源类型</span><span class="sxs-lookup"><span data-stu-id="78dba-103">windows10XCustomSubjectAlternativeName resource type</span></span>

<span data-ttu-id="78dba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78dba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78dba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78dba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78dba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78dba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78dba-107"> (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型</span><span class="sxs-lookup"><span data-stu-id="78dba-107">Base Profile Type for Authentication Certificates (SCEP or PFX Create)</span></span>

## <a name="properties"></a><span data-ttu-id="78dba-108">属性</span><span class="sxs-lookup"><span data-stu-id="78dba-108">Properties</span></span>
|<span data-ttu-id="78dba-109">属性</span><span class="sxs-lookup"><span data-stu-id="78dba-109">Property</span></span>|<span data-ttu-id="78dba-110">类型</span><span class="sxs-lookup"><span data-stu-id="78dba-110">Type</span></span>|<span data-ttu-id="78dba-111">描述</span><span class="sxs-lookup"><span data-stu-id="78dba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78dba-112">sanType</span><span class="sxs-lookup"><span data-stu-id="78dba-112">sanType</span></span>|[<span data-ttu-id="78dba-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="78dba-113">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="78dba-114">自定义 SAN 类型。</span><span class="sxs-lookup"><span data-stu-id="78dba-114">Custom SAN Type.</span></span> <span data-ttu-id="78dba-115">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="78dba-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="78dba-116">name</span><span class="sxs-lookup"><span data-stu-id="78dba-116">name</span></span>|<span data-ttu-id="78dba-117">String</span><span class="sxs-lookup"><span data-stu-id="78dba-117">String</span></span>|<span data-ttu-id="78dba-118">自定义 SAN 名称</span><span class="sxs-lookup"><span data-stu-id="78dba-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="78dba-119">关系</span><span class="sxs-lookup"><span data-stu-id="78dba-119">Relationships</span></span>
<span data-ttu-id="78dba-120">无</span><span class="sxs-lookup"><span data-stu-id="78dba-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78dba-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78dba-121">JSON Representation</span></span>
<span data-ttu-id="78dba-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78dba-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCustomSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




