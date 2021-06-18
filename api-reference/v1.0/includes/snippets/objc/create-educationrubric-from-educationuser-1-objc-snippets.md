---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b5cb7d174e09acb9e87e2269a5beb0da3083e1f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992908"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/me/rubrics"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationRubric *educationRubric = [[MSGraphEducationRubric alloc] init];
[educationRubric setDisplayName:@"Example Credit Rubric"];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"This is an example of a credit rubric (no points)"];
[description setContentType: [MSGraphBodyType text]];
[educationRubric setDescription:description];
NSMutableArray *levelsList = [[NSMutableArray alloc] init];
MSGraphRubricLevel *levels = [[MSGraphRubricLevel alloc] init];
[levels setDisplayName:@"Good"];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@""];
[description setContentType: [MSGraphBodyType text]];
[levels setDescription:description];
[levelsList addObject: levels];
MSGraphRubricLevel *levels = [[MSGraphRubricLevel alloc] init];
[levels setDisplayName:@"Poor"];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@""];
[description setContentType: [MSGraphBodyType text]];
[levels setDescription:description];
[levelsList addObject: levels];
[educationRubric setLevels:levelsList];
NSMutableArray *qualitiesList = [[NSMutableArray alloc] init];
MSGraphRubricQuality *qualities = [[MSGraphRubricQuality alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"Argument"];
[description setContentType: [MSGraphBodyType text]];
[qualities setDescription:description];
NSMutableArray *criteriaList = [[NSMutableArray alloc] init];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay's argument is persuasive."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay's argument does not make sense."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
[qualities setCriteria:criteriaList];
[qualitiesList addObject: qualities];
MSGraphRubricQuality *qualities = [[MSGraphRubricQuality alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"Spelling and Grammar"];
[description setContentType: [MSGraphBodyType text]];
[qualities setDescription:description];
NSMutableArray *criteriaList = [[NSMutableArray alloc] init];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay uses proper spelling and grammar with few or no errors."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay has numerous errors in spelling and/or grammar."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
[qualities setCriteria:criteriaList];
[qualitiesList addObject: qualities];
[educationRubric setQualities:qualitiesList];

NSError *error;
NSData *educationRubricData = [educationRubric getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationRubricData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```