---
title: groupPolicyUploadedLanguageFile 资源类型
description: 实体表示管理员上载的 ADML (管理模板语言) XML 文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf5bef8faadac012df13a8a31cfaac3a5dc94ed2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298104"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a><span data-ttu-id="7ff51-103">groupPolicyUploadedLanguageFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ff51-103">groupPolicyUploadedLanguageFile resource type</span></span>

<span data-ttu-id="7ff51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ff51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ff51-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ff51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ff51-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ff51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff51-107">实体表示管理员上载的 ADML (管理模板语言) XML 文件。</span><span class="sxs-lookup"><span data-stu-id="7ff51-107">The entity represents an ADML (Administrative Template language) XML file uploaded by Administrator.</span></span>

## <a name="properties"></a><span data-ttu-id="7ff51-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ff51-108">Properties</span></span>
|<span data-ttu-id="7ff51-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ff51-109">Property</span></span>|<span data-ttu-id="7ff51-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ff51-110">Type</span></span>|<span data-ttu-id="7ff51-111">Description</span><span class="sxs-lookup"><span data-stu-id="7ff51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff51-112">fileName</span><span class="sxs-lookup"><span data-stu-id="7ff51-112">fileName</span></span>|<span data-ttu-id="7ff51-113">String</span><span class="sxs-lookup"><span data-stu-id="7ff51-113">String</span></span>|<span data-ttu-id="7ff51-114">上传的 ADML 文件的文件名。</span><span class="sxs-lookup"><span data-stu-id="7ff51-114">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="7ff51-115">languageCode</span><span class="sxs-lookup"><span data-stu-id="7ff51-115">languageCode</span></span>|<span data-ttu-id="7ff51-116">字符串</span><span class="sxs-lookup"><span data-stu-id="7ff51-116">String</span></span>|<span data-ttu-id="7ff51-117">上传的 ADML 文件的语言代码。</span><span class="sxs-lookup"><span data-stu-id="7ff51-117">The language code of the uploaded ADML file.</span></span>|
|<span data-ttu-id="7ff51-118">content</span><span class="sxs-lookup"><span data-stu-id="7ff51-118">content</span></span>|<span data-ttu-id="7ff51-119">Binary</span><span class="sxs-lookup"><span data-stu-id="7ff51-119">Binary</span></span>|<span data-ttu-id="7ff51-120">已上载的 ADML 文件的内容。</span><span class="sxs-lookup"><span data-stu-id="7ff51-120">The contents of the uploaded ADML file.</span></span>|
|<span data-ttu-id="7ff51-121">id</span><span class="sxs-lookup"><span data-stu-id="7ff51-121">id</span></span>|<span data-ttu-id="7ff51-122">字符串</span><span class="sxs-lookup"><span data-stu-id="7ff51-122">String</span></span>|<span data-ttu-id="7ff51-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ff51-123">Key of the entity.</span></span>|
|<span data-ttu-id="7ff51-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ff51-124">lastModifiedDateTime</span></span>|<span data-ttu-id="7ff51-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ff51-125">DateTimeOffset</span></span>|<span data-ttu-id="7ff51-126">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7ff51-126">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ff51-127">关系</span><span class="sxs-lookup"><span data-stu-id="7ff51-127">Relationships</span></span>
<span data-ttu-id="7ff51-128">无</span><span class="sxs-lookup"><span data-stu-id="7ff51-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ff51-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ff51-129">JSON Representation</span></span>
<span data-ttu-id="7ff51-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ff51-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedLanguageFile",
  "fileName": "String",
  "languageCode": "String",
  "content": "binary",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




