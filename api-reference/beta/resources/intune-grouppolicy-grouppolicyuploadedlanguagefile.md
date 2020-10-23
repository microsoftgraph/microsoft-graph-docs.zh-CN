---
title: groupPolicyUploadedLanguageFile 资源类型
description: 实体表示管理员上载的 ADML (管理模板语言) XML 文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc70d0ff85cebc567b9efc67b87bb57e2e8337fa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707687"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a><span data-ttu-id="10774-103">groupPolicyUploadedLanguageFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="10774-103">groupPolicyUploadedLanguageFile resource type</span></span>

<span data-ttu-id="10774-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10774-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10774-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10774-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10774-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10774-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10774-107">实体表示管理员上载的 ADML (管理模板语言) XML 文件。</span><span class="sxs-lookup"><span data-stu-id="10774-107">The entity represents an ADML (Administrative Template language) XML file uploaded by Administrator.</span></span>

## <a name="properties"></a><span data-ttu-id="10774-108">属性</span><span class="sxs-lookup"><span data-stu-id="10774-108">Properties</span></span>
|<span data-ttu-id="10774-109">属性</span><span class="sxs-lookup"><span data-stu-id="10774-109">Property</span></span>|<span data-ttu-id="10774-110">类型</span><span class="sxs-lookup"><span data-stu-id="10774-110">Type</span></span>|<span data-ttu-id="10774-111">说明</span><span class="sxs-lookup"><span data-stu-id="10774-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10774-112">fileName</span><span class="sxs-lookup"><span data-stu-id="10774-112">fileName</span></span>|<span data-ttu-id="10774-113">String</span><span class="sxs-lookup"><span data-stu-id="10774-113">String</span></span>|<span data-ttu-id="10774-114">上传的 ADML 文件的文件名。</span><span class="sxs-lookup"><span data-stu-id="10774-114">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="10774-115">languageCode</span><span class="sxs-lookup"><span data-stu-id="10774-115">languageCode</span></span>|<span data-ttu-id="10774-116">String</span><span class="sxs-lookup"><span data-stu-id="10774-116">String</span></span>|<span data-ttu-id="10774-117">上传的 ADML 文件的语言代码。</span><span class="sxs-lookup"><span data-stu-id="10774-117">The language code of the uploaded ADML file.</span></span>|
|<span data-ttu-id="10774-118">content</span><span class="sxs-lookup"><span data-stu-id="10774-118">content</span></span>|<span data-ttu-id="10774-119">Binary</span><span class="sxs-lookup"><span data-stu-id="10774-119">Binary</span></span>|<span data-ttu-id="10774-120">已上载的 ADML 文件的内容。</span><span class="sxs-lookup"><span data-stu-id="10774-120">The contents of the uploaded ADML file.</span></span>|
|<span data-ttu-id="10774-121">id</span><span class="sxs-lookup"><span data-stu-id="10774-121">id</span></span>|<span data-ttu-id="10774-122">String</span><span class="sxs-lookup"><span data-stu-id="10774-122">String</span></span>|<span data-ttu-id="10774-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="10774-123">Key of the entity.</span></span>|
|<span data-ttu-id="10774-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10774-124">lastModifiedDateTime</span></span>|<span data-ttu-id="10774-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10774-125">DateTimeOffset</span></span>|<span data-ttu-id="10774-126">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="10774-126">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10774-127">关系</span><span class="sxs-lookup"><span data-stu-id="10774-127">Relationships</span></span>
<span data-ttu-id="10774-128">无</span><span class="sxs-lookup"><span data-stu-id="10774-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10774-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10774-129">JSON Representation</span></span>
<span data-ttu-id="10774-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10774-130">Here is a JSON representation of the resource.</span></span>
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





