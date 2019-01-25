---
title: educationPowerSchoolDataProvider 资源
description: 用于 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510461"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="02abd-103">educationPowerSchoolDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="02abd-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02abd-104">用于[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="02abd-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="02abd-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="02abd-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="02abd-106">属性</span><span class="sxs-lookup"><span data-stu-id="02abd-106">Properties</span></span>

| <span data-ttu-id="02abd-107">属性</span><span class="sxs-lookup"><span data-stu-id="02abd-107">Property</span></span> | <span data-ttu-id="02abd-108">类型</span><span class="sxs-lookup"><span data-stu-id="02abd-108">Type</span></span> | <span data-ttu-id="02abd-109">说明</span><span class="sxs-lookup"><span data-stu-id="02abd-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="02abd-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="02abd-110">**connectionUrl**</span></span> | <span data-ttu-id="02abd-111">String</span><span class="sxs-lookup"><span data-stu-id="02abd-111">String</span></span> | <span data-ttu-id="02abd-112">连接到 PowerSchool 实例 URL。</span><span class="sxs-lookup"><span data-stu-id="02abd-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="02abd-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="02abd-113">**clientId**</span></span> | <span data-ttu-id="02abd-114">String</span><span class="sxs-lookup"><span data-stu-id="02abd-114">String</span></span> |  <span data-ttu-id="02abd-115">用于连接到 PowerSchool 客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="02abd-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="02abd-116">client_secret</span><span class="sxs-lookup"><span data-stu-id="02abd-116">**clientSecret**</span></span> | <span data-ttu-id="02abd-117">String</span><span class="sxs-lookup"><span data-stu-id="02abd-117">String</span></span> |  <span data-ttu-id="02abd-118">客户端机密进行身份验证与 PowerSchool 实例的连接。</span><span class="sxs-lookup"><span data-stu-id="02abd-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="02abd-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="02abd-119">**schoolsIds**</span></span> | <span data-ttu-id="02abd-120">String 集合</span><span class="sxs-lookup"><span data-stu-id="02abd-120">String collection</span></span> |  <span data-ttu-id="02abd-121">学校同步的列表。</span><span class="sxs-lookup"><span data-stu-id="02abd-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="02abd-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="02abd-122">**schoolYear**</span></span> | <span data-ttu-id="02abd-123">String</span><span class="sxs-lookup"><span data-stu-id="02abd-123">String</span></span> |  <span data-ttu-id="02abd-124">要同步的学校年份。</span><span class="sxs-lookup"><span data-stu-id="02abd-124">The school year to sync.</span></span> |
| <span data-ttu-id="02abd-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="02abd-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="02abd-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="02abd-126">Boolean</span></span> |  <span data-ttu-id="02abd-127">指示源是否有多个标识符是单个学生或教师。</span><span class="sxs-lookup"><span data-stu-id="02abd-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="02abd-128">**自定义项**</span><span class="sxs-lookup"><span data-stu-id="02abd-128">**customizations**</span></span> | [<span data-ttu-id="02abd-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="02abd-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="02abd-130">可选自定义要应用于同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="02abd-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02abd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02abd-131">JSON representation</span></span>
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
