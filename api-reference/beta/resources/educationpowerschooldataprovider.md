---
title: educationPowerSchoolDataProvider 资源
description: 用于在将 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507115"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="edefd-103">educationPowerSchoolDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="edefd-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edefd-104">用于在将[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="edefd-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="edefd-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="edefd-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="edefd-106">属性</span><span class="sxs-lookup"><span data-stu-id="edefd-106">Properties</span></span>

| <span data-ttu-id="edefd-107">属性</span><span class="sxs-lookup"><span data-stu-id="edefd-107">Property</span></span> | <span data-ttu-id="edefd-108">类型</span><span class="sxs-lookup"><span data-stu-id="edefd-108">Type</span></span> | <span data-ttu-id="edefd-109">说明</span><span class="sxs-lookup"><span data-stu-id="edefd-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="edefd-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="edefd-110">**connectionUrl**</span></span> | <span data-ttu-id="edefd-111">字符串</span><span class="sxs-lookup"><span data-stu-id="edefd-111">String</span></span> | <span data-ttu-id="edefd-112">指向 PowerSchool 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="edefd-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="edefd-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="edefd-113">**clientId**</span></span> | <span data-ttu-id="edefd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="edefd-114">String</span></span> |  <span data-ttu-id="edefd-115">用于连接到 PowerSchool 的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="edefd-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="edefd-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="edefd-116">**clientSecret**</span></span> | <span data-ttu-id="edefd-117">字符串</span><span class="sxs-lookup"><span data-stu-id="edefd-117">String</span></span> |  <span data-ttu-id="edefd-118">用于对与 PowerSchool 实例的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="edefd-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="edefd-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="edefd-119">**schoolsIds**</span></span> | <span data-ttu-id="edefd-120">String collection</span><span class="sxs-lookup"><span data-stu-id="edefd-120">String collection</span></span> |  <span data-ttu-id="edefd-121">要同步的学校列表。</span><span class="sxs-lookup"><span data-stu-id="edefd-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="edefd-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="edefd-122">**schoolYear**</span></span> | <span data-ttu-id="edefd-123">字符串</span><span class="sxs-lookup"><span data-stu-id="edefd-123">String</span></span> |  <span data-ttu-id="edefd-124">要同步的学校年。</span><span class="sxs-lookup"><span data-stu-id="edefd-124">The school year to sync.</span></span> |
| <span data-ttu-id="edefd-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="edefd-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="edefd-126">布尔</span><span class="sxs-lookup"><span data-stu-id="edefd-126">Boolean</span></span> |  <span data-ttu-id="edefd-127">指示源是否具有单个学生或教师的多个标识符。</span><span class="sxs-lookup"><span data-stu-id="edefd-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="edefd-128">**操作**</span><span class="sxs-lookup"><span data-stu-id="edefd-128">**customizations**</span></span> | [<span data-ttu-id="edefd-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="edefd-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="edefd-130">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="edefd-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edefd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edefd-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
