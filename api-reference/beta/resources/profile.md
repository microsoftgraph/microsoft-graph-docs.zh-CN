---
title: 配置文件资源类型
description: 表示为用户描述的属性，以及通过 microsoft Graph 在 Microsoft 365 和第三方服务和体验中呈现的共享人员体验。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2e378229e8b001070db274c812cdb307934717cf
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168572"
---
# <a name="profile-resource-type"></a>配置文件资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对租户中的用户进行描述性的属性，例如，周年纪念和教育活动。 这些属性在跨 Microsoft 365 和第三方服务的共享人员体验和通过 Microsoft Graph 的体验中呈现。 

以编程方式，这些属性表示为**配置文件**资源的[关系](#relationships)。 若要获取这些导航属性之一或为用户创建这些属性的实例，请对该属性使用相应的 GET 或 POST 方法（如果适用）。 请参阅下面列出的[方法](#methods)。

## <a name="methods"></a>方法

| 方法                                                                     | 返回类型                                                    | 说明                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [获取个人资料](../api/profile-get.md)                                       | [profile](profile.md)                                          | 读取 profile 对象的属性和关系。                                         |
| [删除个人资料](../api/profile-delete.md)                                 | 无                                                           | 删除**配置文件**对象。                                                                 |
| [列表帐户](../api/profile-list-account.md)                             | [userAccountInformation](useraccountinformation.md)集合 | 获取**userAccountInformation**对象集合。                                          |
| [创建 personAnniversary](../api/profile-post-anniversaries.md)           | [personAnniversary](personanniversary.md)                      | 通过发布到周年纪念集合创建新的**personAnniversary** 。               |
| [列出周年纪念](../api/profile-list-anniversaries.md)                 | [personAnniversary](personanniversary.md)集合           | 获取**personAnniversary**对象集合。                                               |
| [创建 educationalActivity](../api/profile-post-educationalactivities.md) | [educationalActivity](educationalactivity.md)                  | 通过发布到**educationalActivities**集合创建新的**educationalActivity** 。 |
| [列出 educationalActivities](../api/profile-list-educationalactivities.md) | [educationalActivity](educationalactivity.md)集合       | 获取**educationalActivity**对象集合。                                            |
| [创建 itemEmail](../api/profile-post-emails.md)                          | [itemEmail](itememail.md)                                      | 通过发布到电子邮件集合创建新的**itemEmail** 。                              |
| [列出电子邮件](../api/profile-list-emails.md)                               | [itemEmail](itememail.md)集合                           | 获取**itemEmail**对象集合。                                                      |
| [创建 personInterest](../api/profile-post-interests.md)                  | [personInterest](personinterest.md)                            | 通过发布到 "兴趣" 集合创建新的**personInterest** 。                      |
| [列出兴趣](../api/profile-list-interests.md)                         | [personInterest](personinterest.md)集合                 | 获取**personInterest**对象集合。                                                  |
| [创建 languageProficiency](../api/profile-post-languages.md)             | [languageProficiency](languageproficiency.md)                  | 通过发布到语言集合创建新的**languageProficiency** 。                 |
| [列出语言](../api/profile-list-languages.md)                         | [languageProficiency](languageproficiency.md)集合       | 获取**languageProficiency**对象集合。                                             |
| [列出名称](../api/profile-list-names.md)                                 | [contact.personname](personname.md)集合                         | 获取**contact.personname**对象集合。                                                      |
| [创建 Contact.personname](../api/profile-post-names.md)                          | [Contact.personname](personName.md)                                    | 通过发布到名称集合创建新的**contact.personname**对象。                       |
| [列出网站](../api/profile-list-websites.md)                           | [personWebsite](personwebsite.md)集合                   | 获取**personWebsite**对象集合。                                                   |
| [创建 itemPhone](../api/profile-post-phones.md)                          | [itemPhone](itemphone.md)                                      | 通过发布到 "电话" 集合创建新的 itemPhone。                                  |
| [列出电话](../api/profile-list-phones.md)                               | [itemPhone](itemphone.md)集合                           | 获取**itemPhone**对象集合。                                                       |
| [创建 workPosition](../api/profile-post-positions.md)                    | [workPosition](workposition.md)                                | 通过发布到 "职位" 集合创建新的 workPosition。                            |
| [列表位置](../api/profile-list-positions.md)                         | [workPosition](workposition.md)集合                     | 获取**workPosition**对象集合。                                                    |
| [创建 projectParticipation](../api/profile-post-projects.md)             | [projectParticipation](projectparticipation.md)                | 通过发布到项目集合创建新的**projectParticipation** 。                 |
| [列出项目](../api/profile-list-projects.md)                           | [projectParticipation](projectparticipation.md)集合     | 获取**projectParticipation**对象集合。                                            |
| [创建 skillProficiency](../api/profile-post-skills.md)                   | [skillProficiency](skillproficiency.md)                        | 通过发布到技能集合创建新的**skillProficiency** 。                       |
| [列表技能](../api/profile-list-skills.md)                               | [skillProficiency](skillproficiency.md)集合             | 获取**skillProficiency**对象集合。                                                |
| [创建 webAccount](../api/profile-post-webaccounts.md)                    | [webAccount](webaccount.md)                                    | 通过发布到 webAccounts 集合创建新的**webAccount** 。                        |
| [列出 webAccounts](../api/profile-list-webaccounts.md)                     | [webAccount](webaccount.md)集合                         | 获取**webAccount**对象集合。                                                      |
| [创建 personWebsite](../api/profile-post-websites.md)                    | [personWebsite](personwebsite.md)                              | 通过发布到网站集创建新的**personWebsite** 。                        |
| [列出网站](../api/profile-list-websites.md)                           | [personWebsite](personwebsite.md)集合                   | 获取**personWebsite**对象集合。                                                   |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id            |字符串       | 只读。  |

## <a name="relationships"></a>关系

| 关系          | 类型                                                         | 说明                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|上级                |[userAccountInformation](useraccountinformation.md)集合| 表示特定绑定到用户帐户的信息。 此为只读属性。 可为 NULL。                                                             |
|周年          |[personAnniversary](personanniversary.md)集合          | 代表与人员关联的有意义的日期的详细信息。 此为只读属性。 可为 NULL。                                                      |
|educationalActivities  |[educationalActivity](educationalactivity.md)集合      | 表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。 此为只读属性。 可为 NULL。|
|电子邮件                 |[itemEmail](itememail.md)集合                          | 表示有关与用户相关联的电子邮件地址的详细信息。 此为只读属性。 可为 NULL。                                           |
|interests              |[personInterest](personinterest.md)集合                | 提供有关用户在各种服务中与其自身关联的兴趣的详细信息。 此为只读属性。 可为 NULL。                |
|languages              |[languageProficiency](languageproficiency.md)集合      | 表示有关用户已添加到其配置文件中的语言的详细信息。 此为只读属性。 可为 NULL。                                   |
|phones                 |[itemPhone](itemphone.md)集合                          | 表示有关与各种服务中的用户关联的电话号码的详细信息。 此为只读属性。 可为 NULL。                           |
|位置              |[workPosition](workposition.md)集合                    | 表示有关与用户配置文件相关联的工作职位的详细信息。 此为只读属性。 可为 NULL。                                    |
|projects               |[projectParticipation](projectparticipation.md)集合    | 表示有关与用户关联的项目的详细信息。 此为只读属性。 可为 NULL。                                                    |
|skills                 |[skillProficiency](skillproficiency.md)集合            | 表示有关与各种服务中的用户相关的技能的详细信息。 此为只读属性。 可为 NULL。                                  |
|webAccounts            |[webAccount](webaccount.md)集合                        | 表示用户已将其添加到其用户配置文件中的 web 帐户。 此为只读属性。 可为 NULL。                               |
|websites               |[personWebsite](personwebsite.md)集合                  | 表示有关与各种服务中的用户相关联的网站的详细信息。 此为只读属性。 可为 Null。                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```

<!--
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
-->


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
